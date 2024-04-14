<template>
  <NavBar></NavBar>
  <div id="columns">
    <figure @click="redirectToPage('/gallerie/artober-2023-p1')">
      <img src="@/assets/logo_artefrei.png" alt="test" />
      <figcaption>Art'Ober 2023 - Partie 1</figcaption>
      <p>📅 | 01/10/2023 ➡ 10/10/2023</p>
    </figure>

    <figure @click="redirectToPage('/gallerie/artober-2023-p2')">
      <img src="@/assets/logo_artefrei.png" alt="test" />
      <figcaption>Art'Ober 2023 - Partie 2</figcaption>
      <p>📅 | 11/10/2023 ➡ 20/10/2023</p>
    </figure>

    <figure @click="redirectToPage('/gallerie/artober-2023-p3')">
      <img src="@/assets/logo_artefrei.png" alt="test" />
      <figcaption>Art'Ober 2023 - Partie 3</figcaption>
      <p>📅 | 21/10/2023 ➡ 31/10/2023</p>
    </figure>
  </div>
  <FooTer></FooTer>
</template>
    
<script>
import NavBar from "./NavBar.vue";
import FooTer from "./FooTer.vue";

export default {
  components: {
    NavBar,
    FooTer,
  },
  data() {
    return {
      showMobileMenu: false,
    };
  },
  methods: {
    showMenu() {
      this.showMobileMenu = !this.showMobileMenu;
    },
    showSettings() {
      // Handle the settings click event here
    },
    redirectToPage(page) {
      this.$router.push(page); // Redirection vers la page spécifiée
    },
  },
};
</script>
  
  <style lang="scss" scoped>
@font-face {
  font-family: "BebasNeue";
  src: url("@/assets/BebasNeue-Regular.woff2") format("woff2"),
    url("@/assets/BebasNeue-Regular.ttf") format("truetype");
}

@font-face {
  font-family: "Amarillo";
  src: url("@/assets/Amarillo.ttf") format("truetype");
}

.search-container {
  margin-top: 250px;
  display: flex;
  align-items: center;
  justify-content: center; /* Centrer horizontalement */
  margin-bottom: -100px;
}

input[type="text"] {
  padding: 7.5px;
  border: 1px solid #ccc;
  border-radius: 5px 0 0 5px;
  font-size: 20px;
}

button {
  padding: 8.5px 20px;
  background-color: #00adef;
  color: white;
  border: none;
  border-radius: 0 5px 5px 0;
  cursor: pointer;
  font-size: 20px;
}

button:hover {
  background-color: #00adef;
}

input[type="text"]:focus {
  outline: none;
  border-color: #00adef;
}

#columns {
  display: grid;
  flex-wrap: wrap;
  flex-direction: row;
  justify-content: space-between;
  width: 90%;
  max-width: 1100px;
  margin-left: auto;
  margin-right: auto;
  margin-top: 200px;
  padding: 0 20px;
  box-sizing: border-box;
  grid-template-columns: repeat(3, 1fr);
}

div#columns figure {
  margin-bottom: 30px; /* Espacement entre les lignes */
  margin-right: 30px;
  margin-left: 30px;
  background-color: #00adef;
  background-image: linear-gradient(160deg, #00adef 0%, #ffffff 100%);
  box-shadow: 0 5px 20px rgba(1, 1, 1, 0.2);
  padding: 15px;
  padding-bottom: 10px;
  transition: opacity 0.4s ease-in-out;
  display: inline-block;
  border-radius: 20px;
  margin-bottom: 40px;
}

div#columns figure img {
  width: auto;
  height: 100px;
  padding-bottom: 15px;
  margin-left: 88px;
  margin-right: auto;
  margin-bottom: 5px;
}

div#columns figure figcaption {
  font-size: 28px;
  color: #000000;
  background-color: #ffffff;
  border-radius: 20px;
  line-height: 1.5;
  font-family: "BebasNeue", sans-serif;
  padding: 10px;
  margin-left: 5px;
  margin-right: 5px;
  text-align: center;
}

div#columns figure p {
  font-size: 18px;
  color: #000000;
  line-height: 1.5;
  font-family: "BebasNeue", sans-serif;
  padding: 2px;
  margin-left: 5px;
  margin-right: 5px;
  text-align: left;
  font-family: "BebasNeue", sans-serif;
  margin-top: 40px;
}

div#columns small {
  font-size: 1rem;
  float: right;
  text-transform: uppercase;
  color: #000000;
}

div#columns small a {
  color: #000000;
  text-decoration: none;
  transition: 0.4s color;
}

figure:hover {
  cursor: pointer;
}

div#columns:hover figure:not(:hover) {
  opacity: 0.4;
}

@media screen and (max-width: 1600px) {
  #columns {
    display: grid;
    grid-template-columns: repeat(1, 1fr);
    margin-left: auto !important;
    margin-right: auto !important;
  }
  #columns figure {
    width: 100%;
  }
  div#columns figure {
    margin-left: -20px;
    flex-basis: calc(
      100% - 20px
    ); /* Sur un écran étroit, chaque figure occupe toute la largeur */
  }

  div#columns figure img {
    display: block;
    margin-left: auto;
    margin-right: auto;
  }
}
</style>