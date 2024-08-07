<template>

    <main class="generator">

        <section class="input-generator">
  
            <label for="widthChoice">Width</label>
            <input type="number"  id="widthChoice" v-model.number="width.v">

            <label for="qrcode-value">Digit a text for a Qrcode:</label>
    
            <input v-model="inputvalue" id="qrcode-value" type="text"  placeholder="Text for Qrcode Generation">
            
            <button type="button" @click="generateQrCode">Generate</button>

        </section>

        <section v-html="qrcode" class="qrcode-generated">
            
        </section>

    </main>

</template>

<script setup>
    import Qrcode from "qrcode"
    import {  reactive, ref} from "vue"

    
    let inputvalue = ref("")
    let qrcode = ref("")
    let width = reactive({v: 370})
    

    

    const generateQrCode =  (async () => {
        
        qrcode.value = await Qrcode.toString(inputvalue.value, {width: width.v}).then(value => value)
        

    })


    //console.log(Qrcode.toCanvas("adae"))

        

</script>

<style scoped>

    @import "../assets/generatorStyle.css"

</style>