<template>
  <div class='knight-component'>
    <div class='knight' :class='state'></div>
  </div>
</template>

<script>
export default {
  props: ['state']
}
</script>

<style scoped>
.walk {
  animation: walk .65s steps(7) infinite;
  background: url('../assets/knight-walk.png') -10px -10px;
  height: 1057px;
  width: 1478px;
}

@keyframes walk {
  100% {
    background-position: -10486px;
  }
}

.attack {
  animation: attack .65s steps(8) infinite;
  background: url('../assets/knight-attack.png') -10px -10px;
  height: 1104px;
  width: 1635px;
}

@keyframes attack {
  100% {
    background-position: -13240px;
  }
}

.die {
  animation: die .65s steps(7) infinite;
  background: url('../assets/knight-die.png') -10px -10px;
  height: 1369px;
  width: 1841px;
}

@keyframes die {
  100% {
    background-position: -13027px;
  }
}

.hurt {
  animation: hurt .65s steps(7) infinite;
  background: url('../assets/knight-hurt.png') -10px -10px;
  height: 1057px;
  width: 1478px;
}

@keyframes hurt {
  100% {
    background-position: -11109px;
  }
}
</style>
