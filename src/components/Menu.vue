<template>

    <nav >


        <ul >

            <li><RouterLink to="generator">Generator</RouterLink></li>
            <li><RouterLink to="about">About</RouterLink></li>

        </ul>

    </nav>

</template>

<script setup>

    import {RouterLink} from "vue-router"

</script>

<style scoped>

    @import "../assets/headerStyle.css"

</style>