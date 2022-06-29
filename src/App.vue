/* eslint-disable */
<template>
  <v-app>
    <v-app-bar app color="info">
      <v-toolbar-title>THX - Electron</v-toolbar-title>
    </v-app-bar>

    <v-main>
      <v-container>
        <Home/>
      </v-container>
    </v-main>
  </v-app>
  
</template>

<script>

import Home from './components/Home.vue';
export default {
  name: "App",

  components: {
    Home
  },

  data: () => ({
    //
  }),
};
</script>
