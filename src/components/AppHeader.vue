<template>
    <header>
        <div class="headerContainer">
            <div class="logoContainer"><img src="../assets/images/dc-logo.png" alt="Logo DC"></div>
        <ul>
            <li v-for="(item, index) in navItems" :key="index" :class="{active: item.active}">{{item.text}}</li>
        </ul>
        </div>
    </header>
</template>

<script>
export default {
    name: 'AppHeader',
    data(){
        return{
            navItems:[
                {
                    text: "Characters",
                    active: false
                },
                {
                    text: "Comics",
                    active: true
                },
                {
                    text: "Movies",
                    active: false
                },
                {
                    text: "Tv",
                    active: false
                },
                {
                    text: "Games",
                    active: false
                },
                {
                    text: "Collectibles",
                    active: false
                },
                {
                    text: "Videos",
                    active: false
                },
                {
                    text: "Fans",
                    active: false
                },
                {
                    text: "News",
                    active: false
                },
                {
                    text: "Shop",
                    active: false
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
header {
    width: 100%;
    position: fixed;
    top: 0%;
    left: 0%;
    background-color: white;
}
.headerContainer {
    width: 70%;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 120px;
}
img {
    height: 80px;
}
ul {
    height: 100%;
    display: flex;
    justify-content: center;
    gap: 5%;
    list-style: none;
}
li {
    line-height: 125px;
    height: 100%;
    text-transform: uppercase;
    cursor: pointer;
}
.active {
    color: $mainColor;
    border-bottom: 4px solid $mainColor;
    /* box-shadow: 0px 43px 0px 0px white, 0px 50px 0px 0px $mainColor; */
}

</style>
