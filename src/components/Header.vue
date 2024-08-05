<script setup>
    import MenuComponent from "./Menu.vue"
    import {RouterLink} from "vue-router"

</script>

<template>

    <header class="header  ">

        <h1 class="text-white font-bold"><RouterLink to="/">QrCodeGenerator</RouterLink></h1>

        <MenuComponent />

    </header>

</template>

<style scoped>
    @import "../assets/headerStyle.css"
</style>