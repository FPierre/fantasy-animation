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
.idle {
  animation: idle .65s steps(7) infinite;
  background: url('../assets/knight-idle.png') -0 -0;
  height: 1028px;
  width: 1464px;
}

@keyframes idle {
  100% {
    background-position: -10248px;
  }
}

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
  height: 1116px;
  width: 1567px;
}

@keyframes hurt {
  100% {
    background-position: -11109px;
  }
}

.jump {
  animation: jump .65s steps(7) infinite;
  background: url('../assets/knight-jump.png') -10px -10px;
  height: 1375px;
  width: 1586px;
}

@keyframes jump {
  100% {
    background-position: -11242px;
  }
}
</style>
