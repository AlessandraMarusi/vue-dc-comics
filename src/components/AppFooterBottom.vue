<template>
    <section class="footerBottom">
        <div class="footerBottomContainer">
            <button>Sign-up now!</button>
            <div class="socialContainer">
                <span>Follow us</span>
                <ul>
                    <li v-for="(item, index) in socialItems" :key="index">
                        <img :src=item.img alt="">
                    </li>
                </ul>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'AppFooterBottom',
    data(){
        return{
            socialItems:[
                {
                    text: '',
                    img: require("../assets/images/footer-facebook.png")
                },
                {
                    text: '',
                    img: require("../assets/images/footer-twitter.png")
                },
                {
                    text: '',
                    img: require("../assets/images/footer-youtube.png")
                },
                {
                    text: '',
                    img: require("../assets/images/footer-pinterest.png")
                },
                {
                    text: '',
                    img: require("../assets/images/footer-periscope.png")
                },
            ]
        }
    },
    props: {
        msg: String
    }
}
</script>

<style lang="scss" scoped>
@import '../style/variables';
@import '../style/generals';
.footerBottom {
    background-color: $bgColor;

    position: relative;
    z-index: 1;
}
.footerBottomContainer {
    width: 70%;
    height: 100px;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
    button {
        text-transform: uppercase;
        color: white;
        border: 2px solid $mainColor;
        padding: 10px;
        background-color: transparent;
        font-size: 1rem;
        
    }
}
.socialContainer {
    display: flex;
    align-items: center;
    gap: 30px;
    span {
        color: $mainColor;
        text-transform: uppercase;
        font-weight: bolder;
    }
    ul {
        list-style-type: none;
        display: flex;
        gap: 15px;
    }
}
</style>