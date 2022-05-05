<template>
    <div class="jumbotron"></div>
</template>

<script>
export default {
    name:"AppJumbotron",
    props:{
        msg: String
    }
}
</script>

<style lang="scss" scoped>
    .jumbotron {
        background-image: url("../assets/images/jumbotron.jpg");
        height: 400px;
        background-repeat: no-repeat;
        background-size: cover;
        margin-top: 120px;
    }
</style>