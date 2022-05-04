<template>
    <section class="icons">
        <div class="iconsContainer">
        <ul>
            <li v-for="(item, index) in iconItems" :key="index">
                <img :src=item.icon :alt="'Icona di ' + item.text">
                <span>{{item.text}}</span>
            </li>
        </ul>
    </div>
    </section>
    
</template>

<script>
export default {
    name: 'AppIconBar',
    data(){
        return{
            iconItems:[
                {
                    icon: require("../assets/images/buy-comics-digital-comics.png"),
                    text: 'Digital comics'
                },
                {
                    icon: require("../assets/images/buy-comics-merchandise.png"),
                    text: 'Dc merchandise'
                },
                {
                    icon: require("../assets/images/buy-comics-shop-locator.png"),
                    text: 'Subscriptions'
                },
                {
                    icon: require("../assets/images/buy-comics-subscriptions.png"),
                    text: 'Comic shop locator'
                },
                {
                    icon: require("../assets/images/buy-dc-power-visa.svg"),
                    text: 'Dc power visa'
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
.icons {
    background-color: $mainColor;
    color: white;
    height: 200px;
    display: flex;
    align-items: center;
}
.iconsContainer {
    width: 70%;
    margin: 0 auto;
    ul {
        display: flex;
        justify-content: space-around;
        li{
            display: flex;
            align-items: center;
            text-transform: uppercase;
            justify-content: space-around;
            gap: 10px;
        }
    }
    img {
        height: 50px;
        max-width:60px;
    }
}
</style>