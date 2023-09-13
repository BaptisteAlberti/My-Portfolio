<script setup>
import TheWelcome from '../components/TheWelcome.vue'
</script>

<template>
  <main>
    <TheWelcome />
<body>
  <form>
    <label for="fname">First name:</label><br>
    <input type="text" id="fname" name="fname"><br>
    <label for="lname">Last name:</label><br>
    <input type="text" id="lname" name="lname"><br>
    <label for="object">Object</label><br>
    <input type="text" id="object" name="object"><br>
    <label for="message">Message</label><br>
    <input type="text" id="message" name="message"><br>
    <button>Envoyer</button>
  </form>
</body>
  </main>
</template>
