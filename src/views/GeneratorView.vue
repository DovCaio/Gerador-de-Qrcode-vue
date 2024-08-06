<template>

    <main class="generator">

        <section class="input-generator">
  
            <label for="qrcode-value">Digit a text for a Qrcode:</label>
    
            <input v-model="inputvalue" id="qrcode-value" type="text"  placeholder="Text for Qrcode Generation">
            
            <button type="button" >Generate</button>

        </section>

        <section class="qrcode-generated">
            {{ qrcode }}
        </section>

    </main>

</template>

<script setup>
    //import qrcode from "qrcode"
    import {ref} from "vue"

    let inputvalue = ref("")
    

</script>

<style scoped>

    @import "../assets/generatorStyle.css"

</style>