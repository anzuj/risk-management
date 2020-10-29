<template>
  <div id="app">
    <v-app>
      <v-main fluid fill-height>
          <router-view></router-view>
      </v-main>
    </v-app>
  </div>
</template>

<style>
#app {
  font-family: Montserrat, sans-serif;
  background-color: #8eabf5;
  background-image: url("https://www.transparenttextures.com/patterns/back-pattern.png");
  /* This is mostly intended for prototyping; please download the pattern and re-host for production environments. Thank you! */
}
</style>
