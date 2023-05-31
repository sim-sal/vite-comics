<script>
import AppHeader from './components/AppHeader.vue'

export default (await import('vue')).defineComponent({
  components: {
    AppHeader
  }
})

</script>

<template>
  <AppHeader />
</template>

<style lang="scss">
@use './styles/partials/variables.scss' as *;
@use './styles/general.scss' as *;
</style>
