<template>
    <div>
        <div class="contentContainer">
            <h2>!! Content goes here !!</h2>
        </div>
    </div>
</template>

<script>
export default {
    name: 'AppContent',
    props: {
        msg: String
    }
}
</script>

<style lang="scss" scoped>
@import '../style/variables';
@import '../style/generals';
div {
    background-color: $bgColor;
    height: 100px;
    width: 100%;
}
.contentContainer {
    width: 70%;
    margin: 0 auto;
    display: flex;
    align-items: center;
    h2 {
        color: white;
    }
}
</style>