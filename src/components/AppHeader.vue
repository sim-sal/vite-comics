<script>

export default (await import('vue')).defineComponent({
    name: "AppHeader",
})

</script>

<template>
    <header>

        <div>

            <!-- logo -->
            <div id="logo">
                <img src="../assets/img/dc-logo.png" alt="">
            </div>

            <nav>
                <ul>
                    <li>
                        <a href="">
                            link N.
                        </a>
                    </li>
                </ul>
            </nav>

        </div>

    </header>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;
</style>