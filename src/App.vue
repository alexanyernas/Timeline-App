<template>
  <v-app>
    <v-main>
      <!-- <particles /> -->
      <timeline />
      <!-- <message /> -->
    </v-main>
  </v-app>
</template>

<script>
// import Particles from './components/Particles.vue'
import Timeline from './components/Timeline.vue'
import Message from './components/Message.vue'

export default {
  name: 'App',
  components: {
    Timeline,
    // Particles,
    Message
  }
};
</script>

<style>
* 
{
  font-family: 'Poppins', sans-serif;
}

::-webkit-scrollbar 
{
  width: .5rem;
  border-radius: .5rem;
}

::-webkit-scrollbar-thumb 
{
  background-color: #9575CD;
  border-radius: .5rem;
}

::-webkit-scrollbar-thumb:hover
{
  background-color: #BA68C8;
}
</style>