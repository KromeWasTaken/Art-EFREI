<template>
    <NavBar></NavBar>
    <div class="title">Art'OBER 2023 - Partie 2</div>
    <div class="subtitle">🚧 En cours de travaux 🚧</div>
    <FooTer></FooTer>
  </template>
          
      <script>
  import NavBar from "@/components/NavBar.vue";
  import FooTer from "@/components/FooTer.vue";
  
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
  
  @font-face {
    font-family: "Calluna";
    src: url("https://s3-us-west-2.amazonaws.com/s.cdpn.io/4273/callunasansregular-webfont.woff")
      format("woff");
  }
  
  .title {
    font-family: "BebasNeue", sans-serif;
    margin-top: 250px;
    font-size: 50px;
    text-align: center;
    margin-bottom: -200px;
    span {
      background-color: #fef200;
    }
  }
  
  .subtitle {
    font-family: "BebasNeue", sans-serif;
    margin-top: 250px;
    font-size: 30px;
    text-align: center;
    margin-bottom: -200px;
    span {
      background-color: #fef200;
    }
  }
  
  body {
    background: url(//subtlepatterns.com/patterns/scribble_light.png);
    min-height: 1000px;
    left: 0;
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    background-color: #f0f0f0;
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
    display: flex;
    flex-wrap: wrap;
    flex-direction: row;
    justify-content: space-between;
    width: 90%;
    max-width: 1100px;
    margin: 50px auto;
    margin-top: 200px;
    left: 0;
    margin-bottom: -200px;
  }
  
  div#columns figure {
    position: relative; /* Définir la position relative pour le conteneur */
    width: calc(29%); /* Largeur de chaque figure (33.33% - marge) */
    margin-bottom: 20px; /* Espacement entre les lignes */
    background: #fefefe;
    border: 2px solid #fcfcfc;
    box-shadow: 0 5px 20px rgba(1, 1, 1, 0.2);
    margin: 50px 2px 15px;
    padding: 15px;
    padding-bottom: 10px;
    transition: opacity 0.4s ease-in-out;
    display: inline-block;
    border-radius: 10px;
    transition: 0.3s ease;
  }
  
  div#columns figure:hover {
    transform: scale(1.05);
  }
  
  div#columns figure img {
    width: 100%; /* Utiliser 100% de la largeur du conteneur */
    height: auto; /* Hauteur automatique pour conserver les proportions */
    max-width: 100%; /* Pour s'assurer que l'image ne dépasse pas la largeur spécifiée */
    padding-bottom: 15px;
    margin-bottom: 5px;
  }
  
  div#columns figure figcaption {
    position: absolute; /* Position absolue par rapport au conteneur parent */
    bottom: 0; /* Coller en bas */
    right: 0; /* Coller à droite */
    font-size: 15px;
    color: #000000;
    line-height: 1.5;
    font-family: "BebasNeue", sans-serif;
    padding: 2px;
    margin-left: 5px;
    margin-right: 5px;
    text-align: right;
  }
  
  div#columns figure figcaption:hover {
    text-decoration: underline;
    cursor: pointer;
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
  
  @media screen and (max-width: 1600px) {
    #columns {
      display: flex;
      flex-wrap: wrap;
      flex-direction: column; /* Mettre les conteneurs en colonne */
      justify-content: center; /* Centrer verticalement les conteneurs */
      align-items: center; /* Centrer horizontalement les conteneurs */
    }
    #columns figure {
      width: calc(70%) !important;
    }
  }
  </style>