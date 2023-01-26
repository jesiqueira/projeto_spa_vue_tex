<template>
    <header>Header</header>
    <hr />
    <NavBar />
    <p class="mt-3">{{ info }}</p>
    <hr />
    <button @click="showHIdeEmail" class="btn btn-info mb-2">Clique para contato</button>
    <p v-show="showEmail">ristorante1235@gmail.com</p>
    <p v-show="showEmail"><a class="mt-2" href="tel: 11 999900000">(11) 999900000</a></p>
    <footer>
        Footer
        <MenuImage />
    </footer>
</template>

<script>
import NavBar from './components/NavBar.vue'
import MenuImage from './components/MenuImage.vue'
export default {
    name: 'App',
    components: {
        NavBar,
        MenuImage,
    },
    data() {
        return {
            info: 'Iniciando com CLI Vue',
            showEmail: false,
        }
    },
    methods: {
        showHIdeEmail() {
            this.showEmail = !this.showEmail
        },
    },
}
</script>

<style>
a {
    color: orange
}
</style>
