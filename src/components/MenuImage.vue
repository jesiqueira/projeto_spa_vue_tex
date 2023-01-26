<template>
    <NavBar />
    <p class="p-3"> <a href="#">Aproite nossas promoções</a></p>
    <img :src="urlImage" :alt="AltImage" class="w-25" />
</template>

<script>
import NavBar from './NavBar.vue'
export default {
    name: 'MenuImage',
    data() {
        return {
            urlImage: require('@/assets/produtos/noodles-7390775_1920.jpg'),
            AltImage: 'Pene ao sugo',
        }
    },
    components: {
        NavBar,
    },
}
</script>
<style scoped>
a {
    color: green;
}
</style>
