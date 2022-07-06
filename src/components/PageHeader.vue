<template>
    
    <header>
        <div class="container">
            <div class="logo"><img src="../assets/img/dc-logo.png" alt="" srcset=""></div>
            <nav>
                <ul>
                    <li v-for="link, index in menuLinks" :key="index">
                        <a :href="link.link">{{link.text}}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>

</template>


<script>
export default {
    name: "PageHeader",
    data() {
        return {
            menuLikns: [
                {
                    text: 'characters',
                    link: '#',
                    current: false

                },
                {
                    text: 'comics',
                    link: '#',
                    current: false

                },
                {
                    text: 'movies',
                    link: '#',
                    current: false

                },
                {
                    text: 'tv',
                    link: '#',
                    current: false

                },
                {
                    text: 'games',
                    link: '#',
                    current: false

                },
                {
                    text: 'collectibles',
                    link: '#',
                    current: false

                },
                {
                    text: 'videos',
                    link: '#',
                    current: false

                },
                {
                    text: 'fans',
                    link: '#',
                    current: false

                },
                {
                    text: 'news',
                    link: '#',
                    current: false

                },
                {
                    text: 'shop',
                    link: '#',
                    current: false

                },
                
            ]
        }
    }
}
</script>


<style lang="scss" scoped>
@import "../style/common.scss";

header{
    height: 80px;
    background-color: aqua;
    display: flex;
    align-items: center;

    .container {
        display: flex;
        justify-content: space-between

        
    }

    .logo {
        img {
        width: 60px;
        }

    }

    nav {

    }

    
}

</style>