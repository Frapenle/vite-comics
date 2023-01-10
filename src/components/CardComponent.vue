<template lang="">
    <div class="card">

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
    height: 100px;
    width: calc(100% / 4);
    border: 2px solid red;
    padding: 2rem;
}
</style>