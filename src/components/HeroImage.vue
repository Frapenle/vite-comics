<template lang="">
    <div class="jumbo">
        <img src="../assets/img/jumbotron.jpg" alt="">
    </div>


</template>
<script>
export default {

}
</script>
<style lang="scss">
@use '../styles/partials/variables' as *;

.jumbo {
    height: 300px;
}

img {
    object-fit: cover;
    width: 100%;
    height: 100%;
    object-position: top;
}
</style>