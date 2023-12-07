<template>
    <div>
      <div v-for="player in players" :key="player.id">
      <SinglePlayer v-if="player" :player="player" />
      </div>
    </div>
  </template>
  
  <script>
  import SinglePlayer from './SinglePlayer.vue';
  
  export default {
    name: 'PlayerBox',
    props: {
      players: Array,
    },
    components: {
      SinglePlayer,
    },
  };
  </script>
  
  <style scoped>
  /* Your styles go here */
  </style>
  