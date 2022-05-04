<template>
    <section class="footerTop">
        <img src="../assets/images/dc-logo-bg.png" alt="Logo Dc di background">
        <div class="footerTopContainer">
            <ul>
                <li class="title">Dc comics</li>
                <li v-for="(item, index) in dcComicsLinks" :key="index">{{item.text}}</li>
            </ul>
            <ul>
                <li class="title">Shop</li>
                <li v-for="(item, index) in shopLinks" :key="index">{{item.text}}</li>
            </ul>
            <ul>
                <li class="title">Dc</li>
                <li v-for="(item, index) in dcLinks" :key="index">{{item.text}}</li>
            </ul>
            <ul>
                <li class="title">Sites</li>
                <li v-for="(item, index) in sitesLinks" :key="index">{{item.text}}</li>
            </ul>
        </div>
    </section>
</template>

<script>
export default {
    name: 'AppFooterTop',
    data(){
        return{
            dcComicsLinks:[
                {
                    text: "Characters",
                    link: ""
                },
                {
                    text: "Comics",
                    link: ""
                },
                {
                    text: "Movies",
                    link: ""
                },
                {
                    text: "TV",
                    link: ""
                },
                {
                    text: "Games",
                    link: ""
                },
                {
                    text: "Videos",
                    link: ""
                },
                {
                    text: "News",
                    link: ""
                },
            ],
            shopLinks:[
                {
                    text: "Shop DC",
                    link: ""
                },
                {
                    text: "Shop DC Collectibles",
                    link: ""
                }
            ],
            dcLinks:[
                {
                    text: "Terms Of use",
                    link: ""
                },
                {
                    text: "Privacy policy (New)",
                    link: ""
                },
                {
                    text: "Ad Choices",
                    link: ""
                },
                {
                    text: "Advertising",
                    link: ""
                },
                {
                    text: "Jobs",
                    link: ""
                },
                {
                    text: "Subscriptions",
                    link: ""
                },
                {
                    text: "Talent Workshops",
                    link: ""
                },
                {
                    text: "CPSC Certificates",
                    link: ""
                },
                {
                    text: "Ratings",
                    link: ""
                },
                {
                    text: "Shop Help",
                    link: ""
                },
                {
                    text: "Contact Us",
                    link: ""
                },
            ],
            sitesLinks:[
                {
                    text: "DC",
                    link: ""
                },
                {
                    text: "MAD Magazine",
                    link: ""
                },
                {
                    text: "DC Kids",
                    link: ""
                },
                {
                    text: "DC Universe",
                    link: ""
                },
                {
                    text: "DC Power Visa",
                    link: ""
                },
            ],
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
.footerTop {
    background-image: url("../assets/images/footer-bg.jpg");
    background-repeat: no-repeat;
    background-size: cover;
    img {
        position: absolute;
        right: 20%;
        top: 35%;
    }
}
.footerTopContainer {
    width: 70%;
    height: 400px;
    margin: 0 auto;
    display: flex;
    flex-flow: column wrap;
    align-content: flex-start;
    gap: 10px;
    padding: 50px 0;
    ul {
        list-style: none;
        li {
            color: gray;
        }
        .title {
            color: white;
            text-transform: uppercase;
            padding: 10px 0;
        }
    }
}
</style>