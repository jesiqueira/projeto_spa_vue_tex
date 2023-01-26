<template>
  <h1>Bora codar com {{ vue }} Js 3!</h1>
</template>

<script>
export default {
  name: 'MeuComp',
  data() {
    return {
      vue: 'Vue 4',
    }
  },
  // beforeCreate() {
  //   console.log('beforeCreate', 'Antes de criar a instacia vue')
  //   console.log('Data: ', this.vue)
  //   console.log('DOM: ', this.$refs.title)
  // },
  // created() {
  //   console.log('Create', 'Instancia criada')
  //   console.log('Data: ', this.vue)
  //   console.log('DOM: ', this.$refs.title)
  // },

  // beforeMount() {
  //   console.log('beforeMount:', 'Antes de montar o elemento')
  //   console.log('Data: ', this.vue)
  //   console.log('DOM: ', this.$refs.title)
  // },
  // mounted() {
  //   console.log('Mounted:', 'Montagem concluida')
  //   console.log('Data: ', this.vue)
  //   console.log('DOM: ', this.$refs.title)
  // },
  // beforeUpdate() {
  //   console.log('beforeUpdate:', 'Antes de atualizar dados')
  //   console.log('Data: ', this.vue)
  //   console.log('DOM: ', this.$refs.title)
  // },
  // updated() {
  //   console.log('updated:', 'Atualização concluida')
  //   console.log('Data: ', this.vue)
  //   console.log('DOM: ', this.$refs.title)
  // },
  beforeUnmount() {
    console.log('beforeUnmount:', 'Antes de desmontar o elemento')
    console.log('Data: ', this.vue)
    console.log('DOM: ', this.$refs.title)
  },
  unmounted() {
    console.log('unmounted:', 'Desmontagem concluida')
    console.log('Data: ', this.vue)
    console.log('DOM: ', this.$refs.title)
  },
}
</script>
