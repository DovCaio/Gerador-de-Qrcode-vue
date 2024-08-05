

<template>

    <footer class="footer">



        <div>

            <div>

                <h3 class="">Contact</h3>

                <address>GENERICEMAIL@GENERICDOMINE.com</address>
                <p>PHONE: XXXXX-XXXX</p>

                

            </div>
            
            <nav>
                <h3 class="text">Navigation</h3>
                <ul>

                    <li><RouterLink to="/">Home</RouterLink></li>
                    <li><RouterLink to="/generator">Generator</RouterLink></li>
                    <li><RouterLink to="/about">About</RouterLink></li>
                    

                </ul>

            </nav>

        </div>

        <p>&copy; 2024 Meu Site. Todos os direitos reservados.</p>


    </footer>

</template>


<script setup>
    import { RouterLink } from 'vue-router';

</script>


<style scoped>
    @import "../assets/footerStyle.css"

</style>