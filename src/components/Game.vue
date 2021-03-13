<template>
    <div id="game"></div>
    <button @click="startClient">Start Client</button>
</template>

<script>
import { Client } from "boardgame.io/client";
import { TicTacToe } from "../game/TicTacToe";

export default {
    data() {
        return {
            client: null,
        };
    },

    methods: {
        startClient() {
            console.log(`[Game.vue] - startClient`);
            this.client = Client({ game: TicTacToe });
            this.client.start();
        },
    },
};
</script>
