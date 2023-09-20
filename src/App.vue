<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <header>
    <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="My Portfolio" />

      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
        <RouterLink to="/RessourcesPage">Ressources</RouterLink>
        <RouterLink to="/404Page">404 Page</RouterLink>
        <RouterView />
      </nav>

    </div>
  </header>

  <footer class="footer">
    <a href="https://twitter.com/MrMijumaru" target="_blank"><img src="../public/Images/x-twitter.svg"></a><br>
    <a href="https://www.facebook.com/LeGemeaux" target="_blank"><img src="../public/Images/f-facebook.svg"></a><br>
    <a href="https://www.instagram.com/benvolio_liberta/" target="_blank"><img src="../public/Images/i-instagram.svg"></a><br>
    <a href="https://discord.com/channels/1087359142102061096/1087365206222569522" target="_blank"><img src="../public/Images/d-discord.svg"></a><br>
    <a href="https://www.youtube.com/channel/UCiJNHnKjw3zs4JHkkbrhEbg" target="_blank"><img src="../public/Images/y-youtube.svg"></a><br>
    <a href="https://github.com/BaptisteAlberti" target="_blank"><img src="../public/Images/g-github.svg"></a><br>
    <a href="https://www.linkedin.com/in/baptiste-alberti-b7766a285/" target="_blank"><img src="../public/Images/l-linkedin.svg"></a><br>
  </footer>

</template>

<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
}

.footer {
  width: 10%;
  height: 10%;
  display: flex;
  align-items: center;
  justify-items: center;
}
</style>
