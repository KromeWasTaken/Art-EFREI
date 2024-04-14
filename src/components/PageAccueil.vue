<template>
  <div class="app">
    <NavBar></NavBar>
    <div class="alert__full">
      <div
        class="alert alert--info alert--dismissable"
        role="alert"
        aria-live="polite"
      >
        <button class="alert__close fa fa-times" aria-label="Close">
          <img src="@/assets/cross.png" class="cross_img" alt="Info" />
        </button>
        <p class="alert__heading" role="alertdialog">
          <img src="@/assets/info.png" class="info_img" alt="Info" />
          Ce site internet est optimisé pour tablette et ordinateur portable
          seulement.
        </p>
      </div>
    </div>
    <div class="scrollbar" id="style-8">
      <div class="force-overflow"></div>
    </div>
    <div id="wrapper" data-configuration="1" data-roundness="1">
      <div class="shape"></div>
      <div class="shape"></div>
      <div class="shape"></div>
      <div class="shape"></div>
      <div class="shape"></div>
      <div class="shape"></div>
      <div class="shape"></div>
    </div>
    <div class="title">
      Association d'<span>arts plastiques</span> d'efrei paris
    </div>
    <div class="slider">
      <div class="slide active">
        <img src="@/assets/SFA.jpg" alt="Slide1" />
        <div class="info">
          <p>📅 | 19/03/2024</p>
          <h2>Art'EFREI au SFA 2024</h2>
          <h4>
            On dit bravo à tous les membres d'Art'EFREI qui ont contribué pour
            la création des décors du Spectacle de Fin d'Année ! 👏
          </h4>
        </div>
      </div>
      <div class="slide">
        <img src="@/assets/IntDay.jpg" alt="Slide2" />
        <div class="info">
          <p>📅 | 14/03/2024</p>
          <h2>Art'EFREI à la Journée Internationale</h2>
          <h4>
            Toujours pas assez d'origamis de créé cette année, et c'est pas
            Morgane qui dira le contraire ! 🥳
          </h4>
        </div>
      </div>
      <div class="slide">
        <img src="@/assets/NDE.png" alt="Slide3" />
        <div class="info">
          <p>📅 | 09/12/2023</p>
          <h2>Art'EFREI au Noël des Enfants</h2>
          <h4>
            Au programme, construction de sapins de noël avec des batons en bois
            et atelier coloriage ! 🤩
          </h4>
        </div>
      </div>
      <div class="slide">
        <img src="@/assets/SDA.jpg" alt="Slide4" />
        <div class="info">
          <p>📅 | 14/11/2023</p>
          <h2>Art'EFREI x BDA</h2>
          <h4>
            Art'EFREI participe à la Semaine Des Arts. N'hésitez pas à venir
            nous voir ! 😎
          </h4>
        </div>
      </div>
      <div class="slide">
        <img src="@/assets/JPO.jpeg" alt="Slide5" />
        <div class="info">
          <p>📅 | 21/09/2023</p>
          <h2>Art'EFREI à la Journée Associative</h2>
          <h4>
            Merci à tous ceux qui sont passé faire un dessin ! La fresque pour
            le WEI a été rentabilisé ! 🤣
          </h4>
        </div>
      </div>
      <div class="navigation">
        <img src="@/assets/chevron-gauche.png" class="prev-btn" alt="gauche" />
        <img src="@/assets/chevron-droite.png" class="next-btn" alt="droite" />
      </div>

      <div class="navigation-visibility">
        <div class="slide-icon active"></div>
        <div class="slide-icon"></div>
        <div class="slide-icon"></div>
        <div class="slide-icon"></div>
        <div class="slide-icon"></div>
      </div>
    </div>
    <div class="prez">
      <div class="first">
        <h1>Qui sommes nous ?</h1>
        <p>
          Découvrez une toute nouvelle expérience artistique au cœur d'EFREI
          Paris avec Art'EFREI, l'association d'arts plastiques fraîchement
          créée.<br /><br />
          <span>Que vous soyez débutant ou étudiant expérimenté,</span> notre
          association vous ouvre ses portes pour explorer votre créativité.
          Depuis sa fondation il y a un an, Art'EFREI propose une variété de
          séances hebdomadaires régulières, mettant en avant deux grands axes :
          l'Art du Papier, incluant l'origami et le papercraft, ainsi que le
          Dessin, qu'il soit traditionnel ou digital. <br /><br />Dans le
          contexte difficile de la crise sanitaire du Covid-19, le campus a
          connu une pénurie d'activités artistiques. C'est dans ce cadre que
          nous avons lancé Art'EFREI pour répondre à la demande croissante des
          étudiants. Notre objectif principal est de leur offrir un espace
          d'expression artistique et de développement personnel.
          <span
            >Parcourez notre site pour découvrir nos événements à venir et nos
            projets artistiques.</span
          >
        </p>
      </div>
      <div class="second">
        <h1>En quelques chiffres...</h1>

        <div class="gallery">
          <div class="items">
            <div class="item">
              <div class="item-text">
                <h1>2</h1>
                <p>années d'ancienneté</p>
              </div>
            </div>
            <div class="item">
              <div class="item-text">
                <h1>+50</h1>
                <p>membres</p>
              </div>
            </div>
            <div class="item">
              <div class="item-text">
                <h1>+10</h1>
                <p>événements associatifs</p>
              </div>
            </div>
            <div class="item">
              <div class="item-text">
                <h1>2</h1>
                <p>partenariats</p>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="first">
        <h1>Rejoignez-nous !</h1>
        <div class="container">
          <div class="card">
            <div class="face face1">
              <div class="content">
                <div class="icon">
                  <i class="fa fa-linkedin-square" aria-hidden="true"></i>
                </div>
              </div>
            </div>
            <div class="face face2">
              <div class="content">
                <h3>
                  <a href="https://www.instagram.com/artefrei/" target="_blank"
                    >Instagram</a
                  >
                </h3>
                <p>
                  C'est ici que vous pourrez retrouver les posts des créations
                  des membres d'Art'EFREI dans plusieurs événements prévu dans
                  l'année, <span>notamment l'Art'Ober !</span> Vous pourrez
                  aussi être mis au courant si un évènement futur vous interesse
                  !
                </p>
              </div>
            </div>
          </div>
          <div class="card">
            <div class="face face1">
              <div class="content">
                <div class="icon">
                  <i class="fa fa-twitter-square" aria-hidden="true"></i>
                </div>
              </div>
            </div>
            <div class="face face2">
              <div class="content">
                <h3>
                  <a
                    href="https://discord.com/invite/KFMA3yggab"
                    target="_blank"
                    >Discord</a
                  >
                </h3>
                <p>
                  C'est ici que vous pourrez retrouver les membres d'Art'EFREI
                  et discuter avec eux ! Pleins de salons textuels sont mis à
                  disposition pour critiquer les oeuvres de chacun,
                  <span>échanger sur des astuces de création</span> ou même
                  faire des suggestions quant à l'avenir de l'association !
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <FooTer></FooTer>
  </div>
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
  },
  mounted() {
    const closeButton = document.querySelector(".alert__close");
    const alertFull = document.querySelector(".alert__full");

    closeButton.addEventListener("click", () => {
      alertFull.style.display = "none";
    });

    const slider = document.querySelector(".slider");
    const nextBtn = document.querySelector(".next-btn");
    const prevBtn = document.querySelector(".prev-btn");
    const slides = document.querySelectorAll(".slide");
    const slideIcons = document.querySelectorAll(".slide-icon");
    const numberOfSlides = slides.length;
    var slideNumber = 0;
    const wrapper = document.getElementById("wrapper");

    const rand = (min, max) =>
      Math.floor(Math.random() * (max - min + 1) + min);

    const uniqueRand = (min, max, prev) => {
      let next = prev;

      while (prev === next) next = rand(min, max);

      return next;
    };

    const combinations = [
      { configuration: 1, roundness: 1 },
      { configuration: 1, roundness: 2 },
      { configuration: 1, roundness: 4 },
      { configuration: 2, roundness: 2 },
      { configuration: 2, roundness: 3 },
      { configuration: 3, roundness: 3 },
    ];

    let prev = 0;

    setInterval(() => {
      const index = uniqueRand(0, combinations.length - 1, prev),
        combination = combinations[index];

      wrapper.dataset.configuration = combination.configuration;
      wrapper.dataset.roundness = combination.roundness;

      prev = index;
    }, 3000);

    //image slider next button
    nextBtn.addEventListener("click", () => {
      slides.forEach((slide) => {
        slide.classList.remove("active");
      });
      slideIcons.forEach((slideIcon) => {
        slideIcon.classList.remove("active");
      });

      slideNumber++;

      if (slideNumber > numberOfSlides - 1) {
        slideNumber = 0;
      }

      slides[slideNumber].classList.add("active");
      slideIcons[slideNumber].classList.add("active");
    });

    //image slider previous button
    prevBtn.addEventListener("click", () => {
      slides.forEach((slide) => {
        slide.classList.remove("active");
      });
      slideIcons.forEach((slideIcon) => {
        slideIcon.classList.remove("active");
      });

      slideNumber--;

      if (slideNumber < 0) {
        slideNumber = numberOfSlides - 1;
      }

      slides[slideNumber].classList.add("active");
      slideIcons[slideNumber].classList.add("active");
    });

    //image slider autoplay
    var playSlider;

    var repeater = () => {
      playSlider = setInterval(function () {
        slides.forEach((slide) => {
          slide.classList.remove("active");
        });
        slideIcons.forEach((slideIcon) => {
          slideIcon.classList.remove("active");
        });

        slideNumber++;

        if (slideNumber > numberOfSlides - 1) {
          slideNumber = 0;
        }

        slides[slideNumber].classList.add("active");
        slideIcons[slideNumber].classList.add("active");
      }, 4000);
    };
    repeater();

    //stop the image slider autoplay on mouseover
    slider.addEventListener("mouseover", () => {
      clearInterval(playSlider);
    });

    //start the image slider autoplay again on mouseout
    slider.addEventListener("mouseout", () => {
      repeater();
    });
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

// Alert

$info-color: #176799;
$info-background: #d9f0ff;
$info-border-color: #8ac0c4;

@mixin hide-text {
  text-indent: 100%;
  white-space: nowrap;
  overflow: hidden;
}

.cross_img {
  width: 20px;
  height: 20px;
  margin-right: 6px;
  transition: transform 0.3s ease; /* Animation de transition de 0.3s avec une courbe d'accélération */
  &:hover {
    transform: scale(
      1.2
    ); /* Augmente légèrement la taille de l'image au survol */
  }
}

.info_img {
  width: 20px;
  height: 20px;
}

.alert {
  width: 100%;
  position: relative;
  margin-top: 170px;
  margin-bottom: -150px;
  padding: 0.8em 0;
}

.alert__heading {
  margin: 0;
  width: 100%;
}

.alert__content {
  margin: 1em 0 0;
}

.alert--info {
  // border: 1px solid $info-border-color;
  background: $info-background;
  color: $info-color;
  font-family: "Inter", sans-serif;

  .alert__close:focus {
    outline: 2px solid $info-color;
  }
}

.alert--dismissable {
  .alert__close {
    padding: 0;
    border: 0;
    background: none;
    float: right;

    font-size: 1em;
    line-height: 1;
    color: inherit;
    cursor: pointer;

    // // @include hide-text;
    // &:before {
    //   content: '\f00d';
    //   font-family: 'font-awesome';
    // }
  }

  &:after {
    content: "";
    display: table;
    clear: both;
  }
}

.container {
  width: auto;
  position: relative;
  display: flex;
  justify-content: center;
  margin-top: -50px;
}

.container .card {
  position: relative;
  border-radius: 10px;
  margin: 30px;
}

.container .card .icon {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  transition: 0.7s;
  z-index: 1;
  box-shadow: 0 5px 20px rgba(1, 1, 1, 0.2);
  border-top-left-radius: 20px;
  border-top-right-radius: 20px;
  border-bottom-left-radius: 20px;
  border-bottom-right-radius: 20px;
}

.container .card:nth-child(1) .icon {
  background-image: url("@/assets/insta_test.png");
}

.container .card:nth-child(2) .icon {
  background-image: url("@/assets/discord_test.png");
}

.container .card .icon .fa {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  font-size: 80px;
  transition: 0.7s;
  color: #fff;
}

.content {
  h3 {
    color: #ec008b !important;
    font-family: "BebasNeue", sans-serif;
  }
  h3:hover {
    text-decoration: underline;
  }
  p {
    font-family: "Inter", sans-serif !important;
    text-align: justify !important;
  }
  span {
    background-color: #fef200;
  }
}

.container .card .face {
  width: 600px;
  height: 300px;
  transition: 0.5s;
}

.container .card .face.face1 {
  position: relative;
  background: #333;
  display: flex;
  justify-content: center;
  align-items: center;
  z-index: 1;
  transform: translateY(100px);
  border-top-left-radius: 20px;
  border-top-right-radius: 20px;
  border-bottom-left-radius: 20px;
  border-bottom-right-radius: 20px;
}

.container .card:hover .face.face1 {
  background: #fff;
  transform: translateY(0px);
  border-top-left-radius: 20px;
  border-top-right-radius: 20px;
  border-bottom-left-radius: 0px;
  border-bottom-right-radius: 0px;
}

.container .card .face.face1 .content {
  opacity: 1;
  transition: 0.5s;
}

.container .card:hover .face.face1 .content {
  opacity: 1;
}

.container .card .face.face1 .content i {
  max-width: 100px;
}

.container .card .face.face2 {
  position: relative;
  background: #fff;
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 20px;
  box-sizing: border-box;
  box-shadow: 0 5px 20px rgba(1, 1, 1, 0.2);
  transform: translateY(-200px);
  border-bottom-left-radius: 20px;
  border-bottom-right-radius: 20px;
  border-top-left-radius: 20px;
  border-top-right-radius: 20px;
}

.container .card:hover .face.face2 {
  transform: translateY(0);
  border-top-left-radius: 0px;
  border-top-right-radius: 0px;
}

.container .card .face.face2 .content p {
  margin-top: 10px;
  margin-left: 15px;
  margin-right: 15px;
  padding: 0;
  text-align: center;
  color: #414141;
}

.container .card .face.face2 .content h3 {
  margin: 0 0 10px 0;
  padding: 0;
  color: #fff;
  font-size: 24px;
  text-align: center;
  color: #414141;
}

.container a {
  text-decoration: none;
  color: #414141;
}

#app {
  display: flex;
  flex-direction: column;
  align-items: center; /* Aligner les éléments horizontalement */
}

#wrapper {
  aspect-ratio: 1.618;
  width: 90vmin;
  position: relative;
  margin-top: 200px; /* Ajoutez une marge en haut pour l'espace entre le navbar */
  margin-bottom: -180px; /* Ajoutez une marge en bas pour l'espace */
  margin-left: auto;
  margin-right: auto;
}

#wrapper > .shape {
  height: 30%;
  width: 30%;
  background-color: rgba(255 255 255 / 5%);
  position: absolute;
  transition: left, top, height, width, border-radius;
  transition-duration: 750ms;
  transition-timing-function: ease-in-out;
}

#wrapper > .shape:nth-child(1) {
  background-color: #ec008b;
  z-index: 2;
}

#wrapper > .shape:nth-child(2) {
  background-color: #fef200;
  z-index: 2;
}

#wrapper > .shape:nth-child(3) {
  background-color: #00adef;
  z-index: 2;
}

#wrapper > .shape:nth-child(4) {
  background-color: #00adef;
  z-index: 2;
}

#wrapper > .shape:nth-child(5) {
  background-color: #ec008b;
  z-index: 2;
}

#wrapper > .shape:nth-child(6) {
  background-color: #fef200;
  z-index: 2;
}

#wrapper[data-configuration="1"] > .shape:nth-child(1) {
  left: 0%;
  top: 0%;
  height: 50%;
  width: 20%;
}

#wrapper[data-configuration="1"] > .shape:nth-child(2) {
  left: 20%;
  top: 0%;
  height: 50%;
  width: 30%;
}

#wrapper[data-configuration="1"] > .shape:nth-child(3) {
  left: 50%;
  top: 0%;
  height: 100%;
  width: 50%;
}

#wrapper[data-configuration="1"] > .shape:nth-child(4) {
  left: 0%;
  top: 50%;
  height: 50%;
  width: 30%;
}

#wrapper[data-configuration="1"] > .shape:nth-child(5) {
  left: 30%;
  top: 50%;
  height: 50%;
  width: 20%;
}

#wrapper[data-configuration="1"] > .shape:nth-child(6) {
  left: 70%;
  top: 50%;
  height: 50%;
  width: 30%;
}

#wrapper[data-configuration="1"] > .shape:nth-child(7) {
  left: 85%;
  top: 75%;
  height: 25%;
  width: 15%;
}

#wrapper[data-configuration="2"] > .shape:nth-child(1) {
  left: 25%;
  top: 20%;
  height: 80%;
  width: 15%;
}

#wrapper[data-configuration="2"] > .shape:nth-child(2) {
  left: 40%;
  top: 20%;
  height: 50%;
  width: 10%;
}

#wrapper[data-configuration="2"] > .shape:nth-child(3) {
  left: 50%;
  top: 0%;
  height: 100%;
  width: 25%;
}

#wrapper[data-configuration="2"] > .shape:nth-child(4) {
  left: 0%;
  top: 0%;
  height: 50%;
  width: 10%;
}

#wrapper[data-configuration="2"] > .shape:nth-child(5) {
  left: 10%;
  top: 0%;
  height: 70%;
  width: 15%;
}

#wrapper[data-configuration="2"] > .shape:nth-child(6) {
  left: 75%;
  top: 10%;
  height: 80%;
  width: 15%;
}

#wrapper[data-configuration="2"] > .shape:nth-child(7) {
  left: 90%;
  top: 40%;
  height: 60%;
  width: 10%;
}

#wrapper[data-configuration="3"] > .shape:nth-child(1) {
  left: 0%;
  top: 16.5%;
  height: 32%;
  width: 20%;
}

#wrapper[data-configuration="3"] > .shape:nth-child(2) {
  left: 20%;
  top: 2.7%;
  height: 55%;
  width: 34%;
}

#wrapper[data-configuration="3"] > .shape:nth-child(3) {
  left: 38%;
  top: 0%;
  height: 100%;
  width: 62%;
}

#wrapper[data-configuration="3"] > .shape:nth-child(4) {
  left: 0%;
  top: 47.3%;
  height: 55%;
  width: 34%;
}

#wrapper[data-configuration="3"] > .shape:nth-child(5) {
  left: 34%;
  top: 56.4%;
  height: 32%;
  width: 20%;
}

#wrapper[data-configuration="3"] > .shape:nth-child(6) {
  left: 66%;
  top: 45%;
  height: 55%;
  width: 34%;
}

#wrapper[data-configuration="3"] > .shape:nth-child(7) {
  left: 80%;
  top: 68%;
  height: 32%;
  width: 20%;
}

#wrapper[data-roundness="1"] > .shape {
  border-radius: 6rem;
}

#wrapper[data-roundness="2"] > .shape {
  border-radius: 0rem;
}

#wrapper[data-roundness="3"] > .shape {
  border-radius: 30rem;
}

#wrapper[data-roundness="4"] > .shape:nth-child(1) {
  border-bottom-left-radius: 10rem;
}

#wrapper[data-roundness="4"] > .shape:nth-child(2) {
  border-radius: 20rem;
}

#wrapper[data-roundness="4"] > .shape:nth-child(3) {
  border-top-right-radius: 12rem;
}

#wrapper[data-roundness="4"] > .shape:nth-child(4) {
  border-top-right-radius: 10rem;
  border-bottom-right-radius: 10rem;
}

#wrapper[data-roundness="4"] > .shape:nth-child(5) {
  border-bottom-left-radius: 10rem;
}

#wrapper[data-roundness="4"] > .shape:nth-child(6) {
  border-top-left-radius: 16rem;
}

#wrapper[data-roundness="4"] > .shape:nth-child(7) {
  border-top-left-radius: 10rem;
}

/* -- YouTube Link Styles -- */

body.menu-toggled > .meta-link > span {
  color: rgb(30, 30, 30);
}

#source-link {
  bottom: 60px;
}

#source-link > i {
  color: rgb(94, 106, 210);
}

#yt-link > i {
  color: rgb(239, 83, 80);
}

.meta-link {
  align-items: center;
  backdrop-filter: blur(3px);
  background-color: rgba(255, 255, 255, 0.05);
  border: 1px solid rgba(255, 255, 255, 0.1);
  border-radius: 6px;
  bottom: 10px;
  box-shadow: 0 5px 20px rgba(1, 1, 1, 0.2);
  cursor: pointer;
  display: inline-flex;
  gap: 5px;
  left: 10px;
  padding: 10px 20px;
  position: fixed;
  text-decoration: none;
  transition: background-color 400ms, border-color 400ms;
  z-index: 10000;
}

.meta-link:hover {
  background-color: rgba(255, 255, 255, 0.1);
  border: 1px solid rgba(255, 255, 255, 0.2);
}

.meta-link > i,
.meta-link > span {
  height: 20px;
  line-height: 20px;
}

.meta-link > span {
  color: white;
  font-family: "Rubik", sans-serif;
  font-weight: 500;
}

/*** fixing bug on reflex ***/

.gallery {
  display: flex;
  align-items: center;
  flex-direction: column;
  position: relative;
  padding-top: 60px;
}

.items {
  margin-top: -100px;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 50px;
  padding: 20px;
}

.item-text h1 {
  font-size: 65px !important;
  position: absolute;
  top: -35px;
  left: 20px;
  font-family: "Amarillo", sans-serif !important;
  text-transform: uppercase;
  color: #ffffff;
}

.item-text p {
  position: absolute;
  font-family: "BebasNeue", sans-serif !important;
  top: 160px;
  left: -10px;
  color: #000000;
  font-size: 24px;
  background-color: #ffffff !important;
  border-radius: 20px !important;
}

@keyframes letter-s {
  0% {
    letter-spacing: 8px;
  }
  100% {
    letter-spacing: 1px;
  }
}

@keyframes lines-s {
  0% {
    width: calc(50% - 175px);
  }
  100% {
    width: calc(50% - 125px);
  }
}

@keyframes hide-s {
  0% {
    opacity: 0.5;
  }
  100% {
    opacity: 0.2;
  }
}

.item {
  flex: 1 1 300px; /* Définit une largeur de base pour chaque élément */
  max-width: 300px; /* Empêche les éléments de dépasser cette largeur */
  width: 300px;
  height: 300px;
  margin: 10px;
  border-radius: 20px;
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
  overflow: hidden;
  position: relative;
  box-shadow: 0 5px 20px rgba(1, 1, 1, 0.2);
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  &:before {
    font-size: 30px;
    line-height: 50px;
    padding-left: 10px;
    mix-blend-mode: exclusion;
    border-radius: 15px;
    content: "";
    position: absolute;
    left: 0;
    top: 0;
    width: 100%;
    height: 100%;
    background-color: #00adef;
    background-image: linear-gradient(160deg, #00adef 0%, #ffffff 100%);
    opacity: 1;
    transition: opacity 0.65s ease 0s;
    box-sizing: border-box;
  }
  &:after {
    content: "";
    background-color: #fff9;
    opacity: 0.6;
    top: 0;
    bottom: 0;
    left: -100%;
    position: absolute;
    width: 5vmin;
    box-shadow: 0 5px 20px #fef200 0.2;
    transform: skew(-20deg);
    transition: all 0.25s ease;
  }
  &:hover {
    &:after {
      left: 400px;
      transition: left 0.5s ease 0s;
    }
  }
}

.first {
  h1 {
    font-family: "Amarillo", sans-serif;
    font-size: 40px;
    margin-left: 20px;
  }
  p {
    border-radius: 10px;
    font-family: "Inter", sans-serif;
    margin-left: 80px;
    margin-right: 40px;
    margin-top: -20px;
    margin-right: 80px;
    padding: 20px;
    background-color: #ffffff;
    text-align: justify;
    font-size: 25px;
  }
  span {
    background-color: #fef200;
  }
}

.second {
  h1 {
    font-family: "Amarillo", sans-serif;
    font-size: 40px;
    margin-left: 20px;
  }
  p {
    border-radius: 10px;
    font-family: "Inter", sans-serif;
    margin-left: 40px;
    margin-right: 40px;
    margin-top: -20px;
    padding: 20px;
    background-color: #fff;
  }
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

/* Begin Slider */
.slider {
  min-height: 40vh;
  position: relative;
  background: #fff;
  width: 90%;
  height: 700px;
  margin: auto;
  overflow: hidden;
  border-radius: 20px;
  box-shadow: 0 5px 20px rgba(1, 1, 1, 0.2);
  margin-bottom: 60px;
  margin-top: 300px;
}

.slider .slide {
  position: absolute;
  width: 100%;
  height: 100%;
  clip-path: circle(0% at 0 50%);
}

.slider .slide.active {
  clip-path: circle(150% at 0 50%);
  transition: 2s;
}

.slider .slide img {
  position: absolute;
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.slider .slide .info {
  position: absolute;
  color: #000;
  background: rgba(255, 255, 255, 0.699);
  width: 33%;
  margin-top: 500px;
  margin-left: 50px;
  padding: 20px;
  border-radius: 20px;
  box-shadow: 0 5px 20px rgba(1, 1, 1, 0.2);
}

.slider .slide .info h2 {
  font-size: 25px;
  font-weight: 800;
  font-family: "Inter", sans-serif;
}

.slider .slide .info h4 {
  font-size: 20px;
  font-weight: 400;
  font-family: "Inter", sans-serif;
  margin-bottom: -10px;
}

.slider .slide .info p {
  font-size: 15px;
  font-family: "BebasNeue", sans-serif;
  margin-bottom: -20px;
  margin-top: -10px;
}

.navigation {
  height: 700px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  opacity: 0;
  transition: opacity 0.5s ease;
  user-select: none;
}

.slider:hover .navigation {
  opacity: 1;
}

.prev-btn,
.next-btn {
  z-index: 999;
  font-size: 2em;
  padding: 10px;
  cursor: pointer;
  background-color: #fef200;
}

.prev-btn {
  border-top-right-radius: 20px;
  border-bottom-right-radius: 20px;
  width: 40px;
}

.next-btn {
  border-top-left-radius: 20px;
  border-bottom-left-radius: 20px;
  width: 40px;
}

.navigation-visibility {
  z-index: 999;
  display: flex;
  justify-content: center;
  user-select: none;
}

.navigation-visibility .slide-icon {
  z-index: 999;
  background: #000000;
  width: 20px;
  height: 10px;
  transform: translateY(-50px);
  margin: 0 6px;
  border-radius: 20px;
  box-shadow: 0 5px 20px rgba(1, 1, 1, 0.2);
}

.navigation-visibility .slide-icon.active {
  background: #ec008b;
}

@media screen and (max-width: 600px) {
  .container {
    display: none;
  }
}
@media screen and (min-width: 601px) and (max-width: 1600px) {
  .slider {
    width: 90%;
  }

  .slider .slide .info {
    position: relative;
    width: 80%;
    margin-left: auto;
    margin-right: auto;
  }
  #wrapper {
    margin-left: auto;
    margin-right: auto;
  }

  .slider .slide .info {
    margin-top: 400px;
  }

  .first h1 {
    font-size: 30px;
  }

  .second h1 {
    font-size: 30px;
    margin-bottom: 50px;
  }

  .first p {
    margin-left: 0px;
    margin-right: 0px;
  }

  .container {
    display: grid;
    width: 80%;
    margin-left: auto !important;
    margin-right: auto !important;
  }
}

/* End Slider */
</style>