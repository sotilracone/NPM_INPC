<template>
  <v-app>
    <v-main>
      <!-- Componente 'Menu' -->
      <Menu />

      <router-view>
        <v-content> </v-content>
      </router-view>

      <!-- Componente 'Footer' -->
      <Footer />
    </v-main>
  </v-app>
</template>

<script>
import Menu from "./components/Menu";
import Footer from "./components/Footer";

export default {
  name: "App",

  components: {
    Menu,
    Footer,
  },

  data: () => ({
    //
  }),
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
 
#nav {
  padding: 30px;
 
  a {
    font-weight: bold;
    color: #2c3e50;
 
    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>


