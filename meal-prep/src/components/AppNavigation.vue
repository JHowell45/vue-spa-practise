<template>
  <v-app-bar app color="brown darken-4" dark>
    <!-- <v-app-bar-nav-icon></v-app-bar-nav-icon>
    <v-toolbar-title>{{ appTitle }}</v-toolbar-title>
    <v-btn text>Menu</v-btn>
    <v-spacer></v-spacer>
    <v-btn text>SIGN IN</v-btn>
    <v-btn color="brown lighten-3">JOIN</v-btn> -->

    <v-app-bar-nav-icon
      class="hidden-md-and-up"
      @click="drawer = !drawer"
    ></v-app-bar-nav-icon>
    <v-spacer class="hidden-md-and-up"></v-spacer>
    <v-toolbar-title>{{ appTitle }}</v-toolbar-title>
    <v-btn text class="hidden-sm-and-down">Menu</v-btn>
    <v-spacer class="hidden-sm-and-down"></v-spacer>
    <v-btn text class="hidden-sm-and-down">SIGN IN</v-btn>
    <v-btn color="brown lighten-3" class="hidden-sm-and-down">JOIN</v-btn>
  </v-app-bar>
</template>

<script>
export default {
  name: "AppNavigation",
  data() {
    return {
      appTitle: "Meal Prep",
      drawer: false
    };
  }
};
</script>

<style scoped></style>
