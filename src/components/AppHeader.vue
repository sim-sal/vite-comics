<script>

export default (await import('vue')).defineComponent({
    name: "AppHeader",
    data() {
        return {
            links: [
                {
                    text: "CHARACTERS",
                    url: "#",
                    current: false,
                },
                {
                    text: "COMICS",
                    url: "#",
                    current: false,
                },
                {
                    text: "MOVIES",
                    url: "#",
                    current: false,
                },
                {
                    text: "TV",
                    url: "#",
                    current: false,
                },
                {
                    text: "GAMES",
                    url: "#",
                    current: false,
                },
                {
                    text: "COLLECTIBLES",
                    url: "#",
                    current: false,
                },
                {
                    text: "VIDEOS",
                    url: "#",
                    current: false,
                },
                {
                    text: "FANS",
                    url: "#",
                    current: false,
                },
                {
                    text: "NEWS",
                    url: "#",
                    current: false,
                },
                {
                    text: "SHOP",
                    url: "#",
                    current: false,
                }
            ]
        }
    }
})

</script>

<template>
    <header>

        <div class="container">

            <div id="header_container">

                <!-- logo -->
                <div id="logo">
                    <img src="../assets/img/dc-logo.png" alt="">
                </div>

                <!-- menù navigazione -->
                <nav>

                    <ul>

                        <li v-for="(link, i) in links" :key="i">
                            <a :class="link.current ? 'active' : ''" :href="link.url">
                                {{ link.text }}
                            </a>
                        </li>

                    </ul>

                </nav>

            </div>

        </div>

    </header>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;
@use '../styles/partials/mixins.scss' as *;

#header_container {
    @include flex-between-center;
    height: 100px;
}

#logo {
    width: 70px
}

ul {
    @include flex-around;
    list-style: none;
    font-size: 12px;

    li {
        margin-left: 20px;

        a {
            text-decoration: none;
            color: black;
            font-weight: bold;

            &.active {
                color: rgb(12, 124, 236);
            }

        }
    }
}
</style>