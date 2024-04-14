<template>
  <div class="showbox">
    <div class="loader">
      <svg class="circular" viewBox="25 25 50 50">
        <circle
          class="path"
          cx="50"
          cy="50"
          r="20"
          fill="none"
          stroke-width="2"
          stroke-miterlimit="10"
        />
      </svg>
    </div>
  </div>
</template>

<script>

</script>

<style scoped>
.loader {
  position: fixed;
  left: 50%;
  top: 50%;
  width: 100px;
  transform: translate(-50%, -50%);
}
.loader:before {
  content: "";
  display: block;
  padding-top: 100%;
}

.circular {
  -webkit-animation: rotate 2s linear infinite;
  animation: rotate 2s linear infinite;
  height: 100%;
  transform-origin: center center;
  width: 100%;
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  margin: auto;
}

.path {
  stroke-dasharray: 1, 200;
  stroke-dashoffset: 0;
  -webkit-animation: dash 1.5s ease-in-out infinite,
    color 6s ease-in-out infinite;
  animation: dash 1.5s ease-in-out infinite, color 6s ease-in-out infinite;
  stroke-linecap: round;
}

@-webkit-keyframes rotate {
  100% {
    transform: rotate(360deg);
  }
}

@keyframes rotate {
  100% {
    transform: rotate(360deg);
  }
}
@-webkit-keyframes dash {
  0% {
    stroke-dasharray: 1, 200;
    stroke-dashoffset: 0;
  }
  50% {
    stroke-dasharray: 89, 200;
    stroke-dashoffset: -35px;
  }
  100% {
    stroke-dasharray: 89, 200;
    stroke-dashoffset: -124px;
  }
}
@keyframes dash {
  0% {
    stroke-dasharray: 1, 200;
    stroke-dashoffset: 0;
  }
  50% {
    stroke-dasharray: 89, 200;
    stroke-dashoffset: -35px;
  }
  100% {
    stroke-dasharray: 89, 200;
    stroke-dashoffset: -124px;
  }
}
@-webkit-keyframes color {
  100%,
  0% {
    stroke: #00ADEF;
  }
  40% {
    stroke: #EC008B;
  }
  66% {
    stroke: #FEF200;
  }
  80%,
  90% {
    stroke: #fff;
  }
}
@keyframes color {
  100%,
  0% {
    stroke: #00ADEF;
  }
  40% {
    stroke: #EC008B;
  }
  66% {
    stroke: #FEF200;
  }
  80%,
  90% {
    stroke: #fff;
  }
}

.showbox {
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  padding: 5%;
}

</style>