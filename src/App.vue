<template>
  <Header-comp />
  <main>
    <router-view></router-view>
    <Footer-comp />
  </main>

    <div class="wrapper">
      <HelloWorld msg="My Portfolio" />

      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
        <RouterLink to="/RessourcesPage">Ressources</RouterLink>
        <RouterView />
      </nav>

    </div>
</template>

<script setup>
  import HeaderComp from './views/Header-comp.vue';
  import FooterComp from './views/Footer-Comp.vue';
  import ContactPage from './views/ContactPage.vue';
  import HomeView from "./views/HomeView.vue";
  import BoutonRetourHaut from './views/BoutonRetourHaut.vue';
  import Bouton_GlobalVue from './views/Bouton_Global.vue';
</script>

<style scoped>

</style>
