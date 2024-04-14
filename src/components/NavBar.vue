<template>
  <div>
    <div class="nav-menu">
      <div class="nav-content" :style="{ height: navMenuHeight }">
        <div class="logo" :style="{ marginTop: logoMarginTop }">
          <RouterLink to="/"
            ><img src="@/assets/logo_artefrei.png" href="/" alt="Logo"
          /></RouterLink>
          <div class="logo_text">
            <img src="@/assets/artefreiBlack.png" alt="Logo_text" />
          </div>
        </div>
        <ul class="nav-items">
          <li><RouterLink to="/" class="a">Accueil</RouterLink></li>
          <li><RouterLink to="/gallerie" class="a">Gallerie</RouterLink></li>
          <li><RouterLink to="/history" class="a">Historique</RouterLink></li>
          <li>
            <RouterLink to="/paint" class="DIY"
              ><img src="@/assets/DIY.png" alt="DIY"
            /></RouterLink>
          </li>
        </ul>
        <div class="navbar-responsive">
          <ul class="navbar-responsive__nav">
            <li><RouterLink to="/" class="a2">Accueil</RouterLink></li>
            <li><RouterLink to="/gallerie" class="a2">Gallerie</RouterLink></li>
            <li><RouterLink to="/history" class="a2">Historique</RouterLink></li>
            <li>
              <RouterLink to="/paint" class="DIY2"
                ><img src="@/assets/DIY.png" alt="DIY2"
              /></RouterLink>
            </li>
          </ul>
        </div>
        <div class="menu_icon" :style="{ marginTop: menuIconMarginTop }" :class="{ active: isResponsiveNavbarVisible }">
          <img
            :src="menuIconImage"
            @click="toggleResponsiveNavbar()"
            alt="menu_icon"
          />
        </div>
      </div>
    </div>
  </div>
</template>
    
  <script>
export default {
  data() {
    return {
      navMenuHeight: "150px", // Définissez la hauteur de base de nav-menu
      isResponsiveNavbarVisible: false, // Nouvelle propriété pour indiquer si la navbar-responsive est visible
    };
  },
  methods: {
    toggleResponsiveNavbar() {
      const navbarResponsive = document.querySelector(".navbar-responsive");
      if (navbarResponsive.style.display === "flex") {
        navbarResponsive.style.display = "none";
        this.navMenuHeight = "150px";
        this.isResponsiveNavbarVisible = false; // Met à jour la propriété
      } else {
        navbarResponsive.style.display = "flex";
        this.navMenuHeight = "500px";
        this.isResponsiveNavbarVisible = true; // Met à jour la propriété
      }
    },
  },
  computed: {
    menuIconImage() {
      // Retourne le chemin de l'image en fonction de l'état de la navbar-responsive
      return this.isResponsiveNavbarVisible
        ? require("@/assets/menu_icon2.png")
        : require("@/assets/menu_icon.png");
    },
    logoMarginTop() {
      // Calcule la marge supérieure du logo en fonction de l'état de la navbar-responsive
      return this.isResponsiveNavbarVisible && this.navMenuHeight !== "150px"
        ? "-350px"
        : "0px"; // Changez "20px" selon votre mise en page
    },
    menuIconMarginTop() {
      // Calcule la marge supérieure du bouton menu_icon en fonction de l'état de la navbar-responsive
      return this.isResponsiveNavbarVisible && this.navMenuHeight !== "150px"
        ? "-350px"
        : "0px"; // Changez "20px" selon votre mise en page
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

//Navbar starts

.navbar-responsive {
  display: none;
  transition: height 0.3s ease; /* Ajout de la transition */
  margin-top: 200px;
}

.navbar-responsive__nav{
  list-style: none !important; /* Retirer les puces */
}

.navbar-responsive .a2{
  font-family: "BebasNeue", sans-serif;
  font-size: 40px;
  padding: 5px 30px;
  text-decoration: none;
  color: #000000;
  transition: font-size 0.3s ease; /* Animation de transition de 0.3s avec une courbe d'accélération */
  &:hover {
    font-size: 50px; /* Augmente légèrement la taille du texte au survol */
  }
}

.DIY2 {
  img {
    width: 300px;
    transition: transform 0.3s ease; /* Animation de transition de 0.3s avec une courbe d'accélération */
    &:hover {
      transform: scale(
        1.2
      ); /* Augmente légèrement la taille de l'image au survol */
    }
  }
}


.logo_text {
  transform: scale(1.8);
  margin-left: 45px;
}

.logo {
  display: flex;
  align-items: center;
  img {
    width: 100px;
    height: auto;
    margin-right: 20px;
    cursor: pointer;
  }
  span {
    align-self: center;
    font-size: 24px;
    font-weight: bold;
    font-family: "Amarillo", sans-serif;
  }
  h3 {
    font-family: "BebasNeue", sans-serif;
    font-size: 40px;
  }
}

.DIY {
  img {
    margin-top: -7px;
    width: 400px;
    transition: transform 0.3s ease; /* Animation de transition de 0.3s avec une courbe d'accélération */
    &:hover {
      transform: scale(
        1.2
      ); /* Augmente légèrement la taille de l'image au survol */
    }
  }
}

.nav-menu {
  background-color: white;
  position: fixed; /* Fixe la navbar en haut de l'écran */
  width: 100%; /* Prend toute la largeur de l'écran */
  z-index: 10000; /* Assure que la navbar reste au-dessus des autres éléments */
  box-shadow: 0 5px 20px rgba(1, 1, 1, 0.2); /* Ombre de 4 pixels vers le bas */
  top: 0; /* Pour s'assurer que la navbar est toujours au sommet de la page */
  margin: 0;
  padding: 0;
  left: 0;
}

.nav-content {
  display: flex;
  justify-content: space-between;
  padding: 10px 30px;
  align-items: center;
  transition: height 0.3s ease; /* Ajout de la transition */
}

.nav-items .a {
  font-family: "BebasNeue", sans-serif;
  font-size: 40px;
  padding: 5px 30px;
  text-decoration: none;
  color: #000000;
  transition: font-size 0.3s ease; /* Animation de transition de 0.3s avec une courbe d'accélération */
  &:hover {
    font-size: 50px; /* Augmente légèrement la taille du texte au survol */
  }
}
.nav-items {
  display: flex;
  justify-content: center;
  align-items: center;
  list-style: none;
  margin: 0;
  overflow: hidden; /* Assure que l'animation ne dépasse pas du conteneur */
  padding: 0;
  li {
    padding: 0 40px;
  }
}
i {
  display: none;
}

@media screen and (max-width: 576px) {
  /* Styles pour les smartphones */
}

@media screen and (min-width: 576px) and (max-width: 992px) {
  /* Styles pour les tablettes */
}

@media screen and (min-width: 992px) and (max-width: 1200px) {
  /* Styles pour les ordinateurs de bureau */
}

@media screen and (min-width: 1200px) {
  /* Styles pour les grands écrans */
}

@media screen and (-webkit-min-device-pixel-ratio: 2),
  (min-resolution: 192dpi) {
  /* Styles pour les écrans haute résolution */
}

@media screen and (min-width: 1599px) {
  .menu_icon {
    display: none !important;
  }

  .navbar-responsive {
    display: none !important;
  }
}

@media screen and (max-width: 1600px) {
  .logo_text,
  .logo span,
  .logo h3,
  .DIY,
  .nav-items {
    display: none;
  }

  .menu_icon {
    display: flex !important;
    width: 50px;
    height: 50px;
    margin-left: auto !important;
    margin-right: 20px !important;
    transition: transform 0.3s ease;
    &:hover {
      transform: scale(
        1.2
      ); /* Augmente légèrement la taille de l'image au survol */
    }
  }

  .logo {
    margin-top: 0px; /* Réaligne le logo vers le haut de la page */
  }

  i {
    display: inline-block; /* Affiche l'icône de menu en mode mobile */
    margin-left: 10px; /* Ajoute un peu d'espace à gauche de l'icône */
    cursor: pointer;
  }

  .nav-items {
    flex-direction: column; /* Affiche les éléments de navigation verticalement */
    text-align: center; /* Centre le texte */
    padding: 0; /* Supprime le rembourrage */
  }

  .nav-items .a {
    font-size: 24px; /* Taille de police réduite */
  }
}

// Navbar ends
</style>