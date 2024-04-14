<template>
  <div class="error">
    <img src="@/assets/thumbnail.png" alt="error404" />
    <h3>Je pense que tu t'es emmêlé les pinceaux...</h3>
    <p>Code d'erreur : 404</p>
    <div class="frame">
      <RouterLink to="/" class="custom-btn btn-3"
        ><span>Retour à l'accueil</span></RouterLink
      >
    </div>
  </div>
</template>
  
  <style scoped>
h3 {
  font-family: "BebasNeue", sans-serif;
  font-size: 30px;
}
p {
  font-family: "Inter", sans-serif;
  font-size: 20px;
}
.frame {
  width: 90%;
  margin: 40px auto;
  text-align: center;
}
button {
  margin: 20px;
}
.custom-btn {
  width: 200px;
  height: 70px;
  color: #fff;
  border-radius: 5px;
  padding: 10px 25px;
  font-family: "Lato", sans-serif;
  font-weight: 500;
  background: transparent;
  cursor: pointer;
  transition: all 0.3s ease;
  position: relative;
  display: inline-block;
  box-shadow: inset 2px 2px 2px 0px rgba(255, 255, 255, 0.5),
    7px 7px 20px 0px rgba(0, 0, 0, 0.1), 4px 4px 5px 0px rgba(0, 0, 0, 0.1);
  outline: none;
  text-decoration: none;
}
.error {
  text-align: center;
}

/* 3 */
.btn-3 {
  background: rgb(0, 172, 238);
  background: linear-gradient(
    0deg,
    rgba(0, 172, 238, 1) 0%,
    rgba(2, 126, 251, 1) 100%
  );
  width: 200px;
  height: 45px;
  line-height: 42px;
  padding: 0;
  border: none;
  margin-top: -20px;
  font-size: 20px;
  text-decoration: none;
}
.btn-3 span {
  font-family: "Inter", sans-serif;
  position: relative;
  display: block;
  width: 100%;
  height: 100%;
  text-decoration: none;
}
.btn-3:before,
.btn-3:after {
  position: absolute;
  content: "";
  right: 0;
  top: 0;
  background: rgba(2, 126, 251, 1);
  transition: all 0.3s ease;
  text-decoration: none;
}
.btn-3:before {
  height: 0%;
  width: 2px;
}
.btn-3:after {
  width: 0%;
  height: 2px;
}
.btn-3:hover {
  background: transparent;
  box-shadow: none;
}
.btn-3:hover:before {
  height: 100%;
}
.btn-3:hover:after {
  width: 100%;
}
.btn-3 span:hover {
  color: rgba(2, 126, 251, 1);
}
.btn-3 span:before,
.btn-3 span:after {
  position: absolute;
  content: "";
  left: 0;
  bottom: 0;
  background: rgba(2, 126, 251, 1);
  transition: all 0.3s ease;
}
.btn-3 span:before {
  width: 2px;
  height: 0%;
}
.btn-3 span:after {
  width: 0%;
  height: 2px;
}
.btn-3 span:hover:before {
  height: 100%;
}
.btn-3 span:hover:after {
  width: 100%;
}

</style>