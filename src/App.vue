<script setup>
import NavbarComponent from "./components/NavbarComponent.vue";
import HeroComponent from "./components/HeroComponent.vue";
import HeroWhoIam from "./components/HeroWhoIam.vue";
import MyTechnologies from "./components/MyTechnologies.vue";
import PlacesThatIWorked from "./components/PlacesThatIWorked.vue";
import HeroFooter from "./components/HeroFooter.vue";
</script>

<template>
  <div id="app">
    <navbar-component />
    <hero-component />
    <hero-who-iam />
    <my-technologies />
    <places-that-i-worked />
    <hero-footer />
  </div>
</template>

<style>
@font-face {
  font-family: "Europa";
  src: local("Europa"), url("./fonts/Europa Regular.ttf") format("truetype");
}

@font-face {
  font-family: "Eurostile";
  font-style: normal;
  font-weight: normal;
  src: local("Eurostile"), url("./fonts/eurostile.TTF") format("truetype");
}
</style>
