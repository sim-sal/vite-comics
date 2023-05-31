<script>
import HelloWorld from './components/HelloWorld.vue'

export default (await import('vue')).defineComponent({
  components: {
    HelloWorld
  }
})

</script>

<template>
  <HelloWorld msg="Vite + Vue" />
</template>

<style lang="scss">
@use './styles/partials/variables.scss' as *;
@use './styles/general.scss' as *;
</style>
