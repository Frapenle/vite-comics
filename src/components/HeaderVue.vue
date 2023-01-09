<template>
    <header>
        <nav>
            <div class="logo">
                <img src="../assets/img/dc-logo.png" alt="DC logo">
            </div>
            <ul>
                <li>menu 1</li>
                <li>menu 2</li>
                <li>menu 3</li>
                <li>menu 4</li>
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

<style scoped>
nav {
    display: flex;
    justify-content: space-between;
}

ul {
    display: flex;
    gap: 2rem;
}
</style>