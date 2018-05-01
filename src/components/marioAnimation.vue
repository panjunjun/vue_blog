<template>
<div class="container">
  <div class="sky">
      <img class="cloud" src="../assets/img/marioAnimation/cloud.png">
      <img class="cloud" src="../assets/img/marioAnimation/cloud.png">
  </div>
  <div class="grass"></div>
  <div class="road">
      <div class="lines"></div>
      <img class="mario" src="../assets/img/marioAnimation/mario.png">
      <img class="luigi" src="../assets/img/marioAnimation/luigi.png">
  </div>
</div>
</template>

<script>

</script>

<style scoped>
.container {
    height: 80%;
    width: 100%;
    overflow: hidden;
    margin: 0;
}

.grass, .sky, .road {
    position: relative;
    width: 100%;
}

.sky {
    height: 40%;
    background: skyblue;
}

.grass {
    height: 30%;
    background: seagreen;
}

.road {
    height: 30%;
    background: dimgray;
    box-sizing: border-box;
    border-top: 10px solid grey;
    border-bottom: 10px solid grey;
}

.lines {
    box-sizing: border-box;
    border: 5px dashed #fff;
    height: 0px;
    width: 100%;
    position: absolute;
    top: 45%;
}

.cloud {
    position: absolute;
}

.mario {
    position: absolute;
    top: -70px;
    left: 0px;
    animation: drive 3s cubic-bezier(0, 1.01, 1, -0.68) infinite both;
}

.luigi {
    position: absolute;
    top: 20px;
    left: 0px;
    animation: drive 4s linear infinite both;
}

.cloud:nth-child(1) {
    width: 200px;
    top: 50px;
    opacity: 0.5;
    animation: wind 80s linear infinite reverse;
}

.cloud:nth-child(2) {
    width: 300px;
    top: 0px;
    animation: wind 50s linear infinite reverse;
}

@keyframes drive {
    from {transform: translateX(-200px)}
    to {transform: translateX(1200px)}
}

@keyframes wind {
    from {left: -300px}
    to {left: 100%}
}
</style>
