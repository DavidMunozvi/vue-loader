<template>
  <div class="home">
      <svg>
        <circle class="stroke-2" r="38" cx="40" cy="40"></circle>
        <circle class="stroke-1" r="38" cx="40" cy="40"></circle>
      </svg>
    </div>
</template>

<script>
export default {
  
}
</script>
<style lang="postcss" scoped>
html body{
  height: 100vh;
  margin: 0;
  padding: 0;
}

.home {
  height: 100vh;
  width: 100%;
  display: flex;
  background-color: darkblue;
  align-items: center;
  justify-content: center;
}

svg {
  width: 80px;
  height: 80px;
  transform: rotateY(-180deg) rotateZ(-90deg);
}

.stroke-1 {
  stroke-dasharray: 240px;
  stroke-dashoffset: 0px;
  stroke-linecap: square;
  stroke-width: 4px;
  stroke: white;
  fill: none;
  animation: countdown 4s linear infinite forwards;
}

.stroke-2 {
  stroke-dasharray: 240px;
  stroke-dashoffset: 0px;
  stroke-linecap: square;
  stroke-width: 4px;
  stroke: rgba(135, 207, 235, 0.274);
  fill: none;
}

@keyframes countdown {
  0% {
    stroke-dashoffset: 0px;
  }
  100% {
    stroke-dashoffset: 240px;
  }

}
</style>
