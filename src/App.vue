<template>
  <v-app>
    <v-main>
      <timeline />
    </v-main>
  </v-app>
</template>

<script>

import Timeline from './components/Timeline.vue'

export default {
  name: 'App',
  components: {
    Timeline
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
  background-color: #E1BEE7;
  border-radius: .5rem;
}

::-webkit-scrollbar-thumb:hover
{
  background-color: #BA68C8;
}
</style>