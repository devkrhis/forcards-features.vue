<template>
  <v-app>
      <HomePage/>
    <v-main>
      <HelloWorld/>
    </v-main>
  </v-app>
</template>

<script>
import HomePage from './components/HomePage.vue';

export default {
  name: 'App',

  components: {
    HomePage,
  },

  data: () => ({
    //
  }),
};
</script>
