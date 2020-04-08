<template>
  <v-app-bar app color="brown darken-4" dark>
    <!-- <v-toolbar-side-icon></v-toolbar-side-icon>
    <v-toolbar-title>{{ appTitle }}</v-toolbar-title>
    <v-btn flat>Menu</v-btn>
    <v-spacer></v-spacer>
    <v-btn flat>SIGN IN</v-btn>
    <v-btn color="brown lighten-3">JOIN</v-btn> -->

    <v-app-bar-side-icon
      class="hidden-md-and-up"
      @click="drawer = !drawer"
    ></v-app-bar-side-icon>
    <v-spacer class="hidden-md-and-up"></v-spacer>
    <v-app-bar-title>{{ appTitle }}</v-app-bar-title>
    <v-btn flat class="hidden-sm-and-down">Menu</v-btn>
    <v-spacer class="hidden-sm-and-down"></v-spacer>
    <v-btn flat class="hidden-sm-and-down">SIGN IN</v-btn>
    <v-btn color="brown lighten-3" class="hidden-sm-and-down">JOIN</v-btn>
  </v-app-bar>
</template>

<script>
export default {
  name: "AppNavigation",
};
</script>

<style scoped></style>
