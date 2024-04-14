<template>
  <div :class="{ 'fade-in': isPageLoaded }">
    <router-view />
    <button
      onclick="window.scrollTo({top: 0, left: 0, behavior: 'smooth'});"
      id="backtotop"
    >
      <img src="@/assets/arrow.png" />
    </button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isPageLoaded: false,
    };
  },
  mounted() {
    // Après le chargement initial de la page
    this.isPageLoaded = true;
    // When the user scrolls down 20px from the top of the document, show the button
    window.onscroll = function () {
      scrollFunction();
    };

    function scrollFunction() {
      if (
        document.body.scrollTop > 20 ||
        document.documentElement.scrollTop > 20
      ) {
        document.getElementById("backtotop").style.display = "block";
      } else {
        document.getElementById("backtotop").style.display = "none";
      }
    }
  },
  watch: {
    $route() {
      // Lorsque la route change
      this.isPageLoaded = false;
      setTimeout(() => {
        this.isPageLoaded = true;
      }, 20); // Ajoutez un délai si nécessaire pour déclencher l'animation
    },
  },
};
</script>

<style lang="scss" scoped>
@keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}

.fade-in {
  animation: fadeIn 0.5s ease-in-out;
}

#backtotop {
  display: none;
  position: fixed;
  bottom: 50px;
  right: 30px;
  z-index: 99;
  font-size: 18px;
  outline: none;
  background-color: #00adef;
  border-radius: 100px;
  border: none;
  cursor: pointer;
  padding: 15px;
  user-select: none;
}

#backtotop img {
  width: 20px;
  height: 20px;
}

#backtotop:hover {
  background-color: #ec008b;
  color: #000000;
}
</style>