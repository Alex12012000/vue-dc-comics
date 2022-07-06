<template>
    <section>
        <div class="container">
            <div class="content">
                <div class="icon-card" v-for="icon, index in iconInfos" :key="index">
                <a :href="icon.link">
                    <img :src="icon.img" :alt="icon.text">
                </a>
                <span>{{icon.text}}</span>
            </div>
            </div>
        </div>
    </section>
</template>


<script>
export default {
    name: "IconInfoSection",
    data() {
        return {
            iconInfos: [
                {
                  img: require ('../assets/img/buy-comics-digital-comics.png'),
                  text: 'digital comics',  
                  link: '#'
                },
                {
                  img: require ('../assets/img/buy-comics-merchandise.png'),
                  text: 'dc merchandise',  
                  link: '#'
                },
                {
                  img: require ('../assets/img/buy-comics-subscriptions.png'),
                  text: 'subscription',
                  link: '#'  
                },
                {
                  img: require ('../assets/img/buy-comics-shop-locator.png'),
                  text: 'comic shop locator',
                  link: '#'  
                },
                {
                  img: require ('../assets/img/buy-dc-power-visa.svg'),
                  text: 'dc power visa',
                  link: '#'  
                },

            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../style/common.scss";
@import "../style/variables.scss";

section {
    background-color: $main_color;
    padding: 20px;
    .content {
        display: flex;
        justify-content: space-between;
        .icon-card {
            padding: 10px;
            display: flex;
            align-items: center;
            justify-content: center;

            span {
                margin: 0 10px;
                font-size: 13px;
                color: white;
                text-transform: uppercase;
            }

            img {
                width: 40px;
            }
        }
    }
}
</style>