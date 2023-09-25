<template>
    <header>
        <nav>
            <ul>
                <RouterLink to="/HomeView"><img src="../components/home.png" alt="Logo bouton acceuil"><p>Home</p></RouterLink>
                <RouterLink to="/RessourcesPage"><img src="../components/projets.png" alt=""><p>Projects</p></RouterLink>
                <RouterLink to="/contact"><img src="../components/mail.png" alt=""><p>Contact</p></RouterLink>
                <RouterView />
            </ul>
        </nav>
    </header>

</template>

<script setup>
import { RouterLink } from 'vue-router';


</script>

<style lang="scss" scoped>
header {
    position: fixed;
    top: 0;
    left: 0;
    z-index: 1;


    width: 100%;
    height: 80px;


    background-color: #36494E;
    border-bottom: 2px solid white;

    display: flex;
    justify-content: center;
    align-items: center;

    nav{
        display: flex;
        justify-content: center;
        align-items: center;

        width: 100%;

        ul {
            width: 100%;
            display: flex;
            justify-content: space-evenly;
            align-items: center;
            a{
                display: flex;
                flex-direction: column;
                justify-content: center;
                align-items: center;
                gap: 2px;
                text-decoration: none;
                padding: 10px;
                border-radius: 20px;
                img{
                    width: 18px;
                    height: 18px;
                }
                &:hover {
                    border-left: 0.7px solid white;
                    border-right: 0.7px solid white;
                    border-radius: 0;
                }

            }
            .router-link-active{
                border-left: 0.7px solid white;
                border-right: 0.7px solid white;
                border-radius: 0;
            }
        }
    }
}

</style>