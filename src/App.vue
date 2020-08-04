<template>
  <div>
    <v-app>
      <Navbar v-if="showNavBar"/>
      <v-main>
        <router-view></router-view>
      </v-main>
    </v-app>
  </div>
</template>

<script>
import Navbar from "./components/Navbar";

export default {
  name: "App",

  components: {
    Navbar,
  },

  data: () => ({
    showNavBar: true,
    app: true
  }),
  mounted() {
    }
};
</script>
