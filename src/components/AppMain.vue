<script>

export default (await import('vue')).defineComponent({
    name: "AppMain",
})

</script>

<template>
    <div id="main-content">
        <div class="container">
            -- CONTENT GOES HERE --
        </div>
    </div>
</template>

<style lang="scss">
@use '../styles/partials/variables.scss' as *;
@use '../styles/partials/mixins.scss' as *;

#main-content {
    background-color: black;
    color: white;
}
</style>