<template>
    <footer>
        <div class="rsociaux">
            <a href="https://twitter.com/MrMijumaru" target="_blank"><img src="../components/Images/x-twitter.svg"></a><br>
            <a href="https://www.facebook.com/LeGemeaux" target="_blank"><img src="../components/Images/f-facebook.svg"></a><br>
            <a href="https://www.instagram.com/benvolio_liberta/" target="_blank"><img src="../components/Images/i-instagram.svg"></a><br>
            <a href="https://discord.com/channels/1087359142102061096/1087365206222569522" target="_blank"><img src="../components/Images/d-discord.svg"></a><br>
            <a href="https://www.youtube.com/channel/UCiJNHnKjw3zs4JHkkbrhEbg" target="_blank"><img src="../components/Images/y-youtube.svg"></a><br>
            <a href="https://github.com/BaptisteAlberti" target="_blank"><img src="../components/Images/g-github.svg"></a><br>
            <a href="https://www.linkedin.com/in/baptiste-alberti-b7766a285/" target="_blank"><img src="../components/Images/l-linkedin.svg"></a><br>
        </div>
        <small>
            Copyright 2023 - Baptiste Alberti <br> <br>
            Dernière mise à jour : <time datetime="2023-10-17">17 octobre 2023</time>
        </small>
    </footer>
</template>

<script setup>

</script>

<style lang="scss" scoped>
footer{
    height: 100px;
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 20px;

    background-color: #1a1a1a;
    padding: 30px;
    .rsociaux{
        background-color: red;
        display: flex;
        justify-content: center;
        align-items: center;
        img{
            height: 50px;
            width: 50px;
            margin: 0 10px;
        }
    }
}

</style>