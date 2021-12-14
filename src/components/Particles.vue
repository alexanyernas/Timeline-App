<template>
  <div class="particles">
    <div id="particles-js"></div>
  </div>
</template>

<script>
import 'particles.js'
import { particlesConfig } from '../config/particlesConfig'
 
export default {
  name: "particles",
  mounted () {
    this.initParticles()
  },
  methods: {
    initParticles () {
      window.particlesJS( "particles-js", particlesConfig )
    }
  }
};
</script>

<style scoped>
.particles
{
    position: absolute;
    height: 100%;
    width: 100%;
}

#particles-js
{
  background: #7E57C2;
  height: 100%;
  width: 100%;
}
</style>
