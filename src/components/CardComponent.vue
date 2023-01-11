<template lang="">
    <div class="card">
        <div class="img">
            <img :src="imgPath" :alt="serie">
        </div>
        <div class="series">
            <h5>{{serie}}</h5>
        </div>
    </div>
</template>
<script>

export default {
    name: 'CardComponent',
    props: [
        "imgPath",
        "price",
        "serie",
        "type"
    ]
}
</script>
<style lang="scss">
.card {
    width: calc(100% / 6 - 1rem);
    margin-bottom: 60px;
    cursor: pointer;
}

.img {
    aspect-ratio: 1;
    width: 100%;
}

img {
    width: 100%;
}

h5 {
    font-weight: 300;
    padding: .7rem 0;
}
</style>