<template lang="">
    <div class="jumbo">
        <img src="../assets/img/jumbotron.jpg" alt="">
        <div class="container">
            <div class="current-series">
                <h4>current series</h4>
            </div>
        </div>
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
    overflow: hidden;
}

.current-series {
    padding: 1rem;
    color: white;
    background-color: $main-color;
}
</style>