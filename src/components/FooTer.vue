<template>
  <div class="footer">
    <div id="button"></div>
    <div id="container">
      <div id="cont">
        <div class="footer_center">
          <p class="copyright-text">
            Copyright &copy; 2024 | Tous droits réservés
            <a href="/" class="test">Art'EFREI</a>
          </p>
          <div class="col-md-4 col-sm-6 col-xs-12">
            <ul class="social-icons">
              <li>
                <a
                  class="youtube"
                  href="https://www.youtube.com/channel/UCSH2SH5ZKSdmS2RLYfLOWjQ"
                  ><img src="@/assets/youtube.png" alt="youtube"
                /></a>
              </li>
              <li>
                <a
                  class="linkedin"
                  href="https://www.linkedin.com/company/art-efrei"
                  ><img src="@/assets/linkedin.png" alt="linkedin"
                /></a>
              </li>
              <li>
                <a class="instagram" href="https://www.instagram.com/artefrei/"
                  ><img src="@/assets/instagram.png" alt="instagram"
                /></a>
              </li>
              <li>
                <a class="discord" href="https://discord.com/invite/KFMA3yggab"
                  ><img src="@/assets/discord.png" alt="discord"
                /></a>
              </li>
              <li>
                <a class="email" href="mailto:artefrei@efrei.net"
                  ><img src="@/assets/email.png" alt="email"
                /></a>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
    <div class="bottom-right-text">Fait avec 💝 & ☕ par <a class="insta_vv" href="https://www.linkedin.com/in/victor-valet">Victor VALET</a></div>
  </div>
</template>

<script>
</script>

<style lang="scss" scoped>
@import url(https://fonts.googleapis.com/css?family=Source+Sans+Pro:300,400);
.test {
  text-decoration: none;
  color: #fff;
  font-weight: bold;
}

.bottom-right-text {
  position: absolute;
  bottom: 0;
  right: 0;
  margin: 10px; /* Ajoutez une marge pour l'espacement */
  font-size: 14px; /* Taille de la police */
  color: #fff; /* Couleur du texte */
  opacity: 0; /* Rendre le texte initialement invisible */
  transition: opacity 0.3s ease; /* Ajouter une transition pour une animation douce */
}

.footer:hover .bottom-right-text {
  opacity: 1; /* Rendre le texte visible lorsque le footer est survolé */
}

.legal {
  text-decoration: none;
  color: #fff;
  text-decoration: underline;
}

.insta_vv {
  font-family: "Inter", sans-serif;
  text-decoration: none;
  color: #fff;
  text-decoration: underline;
}

body {
  font-family: "Source Sans Pro", sans-serif;
  font-weight: 300;
  background-color: lightblue;
  color: #fff;
}
section {
  text-align: center;
}
.footer #button {
  width: 35px;
  height: 35px;
  border: #00adef 12px solid;
  border-radius: 35px;
  margin: 0 auto;
  position: relative;
  -webkit-transition: all 1s ease;
  -moz-transition: all 1s ease;
  -o-transition: all 1s ease;
  -ms-transition: all 1s ease;
  transition: all 1s ease;
}
.footer #button:hover {
  width: 35px;
  height: 35px;
  border: #00adef 12px solid;
  -webkit-transition: all 1s ease;
  -moz-transition: all 1s ease;
  -o-transition: all 1s ease;
  -ms-transition: all 1s ease;
  transition: all 1s ease;
  position: relative;
}
.footer {
  bottom: 0;
  left: 0;
  position: fixed;
  width: 100%;
  height: 2em;
  overflow: hidden;
  margin: 0 auto;
  -webkit-transition: all 1s ease;
  -moz-transition: all 1s ease;
  -o-transition: all 1s ease;
  -ms-transition: all 1s ease;
  transition: all 1s ease;
  z-index: 999;
}
.footer:hover {
  -webkit-transition: all 1s ease;
  -moz-transition: all 1s ease;
  -o-transition: all 1s ease;
  -ms-transition: all 1s ease;
  transition: all 1s ease;
  height: 200px;
}
.footer #container {
  margin-top: 5px;
  width: 100%;
  height: 100%;
  position: relative;
  top: 0;
  left: 0;
  background: #00adef;
}
.footer #cont {
  position: relative;
  top: -45px;
  right: 190px;
  width: 150px;
  height: auto;
  margin: 0 auto;
}
.footer_center {
  width: 500px;
  float: left;
  text-align: center;
}
.footer h3 {
  font-family: "Helvetica";
  font-size: 30px;
  font-weight: 100;
  margin-top: 70px;
  margin-left: 40px;
}

.social-icons {
  padding-left: 0;
  margin-top: 10px;
  list-style: none;
}
.social-icons li {
  display: inline-block;
  margin-bottom: -10px;
  margin-right: 10px;
}
.social-icons li.title {
  margin-right: 15px;
  text-transform: uppercase;
  color: #96a2b2;
  font-weight: 700;
  font-size: 13px;
}
.social-icons a {
  color: #818a91;
  font-size: 16px;
  display: inline-block;
  line-height: 44px;
  width: 44px;
  height: 44px;
  text-align: center;
  margin-right: 8px;
  border-radius: 100%;
  -webkit-transition: all 0.2s linear;
  -o-transition: all 0.2s linear;
  transition: all 0.2s linear;
}
.social-icons a:active,
.social-icons a:focus,
.social-icons a:hover {
  color: #fff;
  background-color: #29aafe;
}
.social-icons.size-sm a {
  line-height: 34px;
  height: 34px;
  width: 34px;
  font-size: 14px;
}
.social-icons a.youtube {
  img {
    width: 50px;
    transition: transform 0.3s ease;
  }
  &:hover {
    transform: scale(1.2);
  }
}

.social-icons a.linkedin {
  img {
    width: 50px;
    transition: transform 0.3s ease;
  }
  &:hover {
    transform: scale(1.2);
  }
}

.social-icons a.instagram {
  img {
    width: 50px;
    transition: transform 0.3s ease;
  }
  &:hover {
    transform: scale(1.2);
  }
}

.social-icons a.discord {
  img {
    width: 50px;
    transition: transform 0.3s ease;
  }
  &:hover {
    transform: scale(1.2);
  }
}

.social-icons a.linktree {
  img {
    width: 50px;
    transition: transform 0.3s ease;
  }
  &:hover {
    transform: scale(1.2);
  }
}

.social-icons a.email {
  img {
    width: 50px;
    transition: transform 0.3s ease;
  }
  &:hover {
    transform: scale(1.2);
  }
}

@media screen and (max-width: 768px) {
}
.copyright-text {
  margin-top: 60px;
  font-family: "Inter", sans-serif;
  color: #fff;
}

</style>