<template>
    <header>
        <nav class="container">
            <div class="logo">
                <img src="../assets/img/dc-logo.png" alt="DC logo">
            </div>
            <ul>
                <li v-for="navItem in navHeader" :class="(navItem.active) ? 'active' : ''"><a href="#">{{
                    navItem.name.toUpperCase()
                }}</a></li>
            </ul>
        </nav>
    </header>
</template>

<script>
export default {
    data() {
        return {
            navHeader: [
                {
                    name: "characters",
                    active: false
                },
                {
                    name: "comics",
                    active: true
                },
                {
                    name: "movies",
                    active: false
                },
                {
                    name: "tv",
                    active: false
                },
                {
                    name: "games",
                    active: false
                },
                {
                    name: "collectibles",
                    active: false
                },
                {
                    name: "videos",
                    active: false
                },
                {
                    name: "fans",
                    active: false
                },
                {
                    name: "news",
                    active: false
                },
                {
                    name: "shop",
                    active: false
                },
            ]
        }
    },
}
</script>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/general.scss' as *;

nav {
    height: 120px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

ul {
    height: 100%;
    align-items: center;
    display: flex;
    gap: 1.5rem;
    font-weight: 500;

    a {
        text-decoration: none;
        color: black;
    }

    li {
        height: 100%;
        display: flex;
        align-items: center;

        &.active {
            color: $main-color;
            border-bottom: 4px solid $main-color;
        }
    }
}

img {
    width: 100%;
}
</style>