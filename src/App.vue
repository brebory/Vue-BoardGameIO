<template>
    <img alt="Vue logo" src="./assets/logo.png" />
    <game></game>
</template>

<script>
import Game from "./components/Game";
export default {
    components: {
        game: Game,
    },
    name: "App",
};
</script>

<style>
#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
}
</style>
