<template>
<TheWelcome ></TheWelcome>
</template>
<script setup>
import { RouterLink, RouterView } from 'vue-router'
import TheWelcome from './views/HomeView.vue';
</script>

<style>
.fondo{
    background-color: black;
    color:white;
}
</style>