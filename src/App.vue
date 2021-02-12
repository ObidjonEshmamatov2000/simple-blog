<template>
  <v-app>
    <TopBar />

    <v-main class="grey lighten-4">
      <router-view></router-view>
    </v-main>
  </v-app>
</template>

<script>
import TopBar from './components/TopBar';


export default {
  name: 'App',

  components: {
    TopBar
  },

  data: () => ({
    //
  }),
};
</script>

