<template>
    
    <!-- Header -->
    <header>
        <div class="container">
            <!-- Header LOGO -->
            <div class="logo"><img src="../assets/img/dc-logo.png" alt="" srcset=""></div>

            <!-- Header NAV -->
            <nav>
                <ul>
                    <li v-for="link, index in menuLinks" :key="index" :class="{ active: link.current}">
                        <a :href="link.link"> {{link.text}} </a>
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
            menuLinks: [
                {
                    text: 'characters',
                    link: '#',
                    current: false

                },
                {
                    text: 'comics',
                    link: '#',
                    current: true

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
@import "../style/variables.scss";

header{
    height: 80px;
    background-color: white;

    .container {
        display: flex;
        justify-content: space-between
    }

    .logo {
        display: flex;
        align-items: center;
        img {
        width: 60px;
        }
    }

    nav {
        ul {
            display: flex;

            li {
                margin: 0 5px;
                line-height: 80px;

                a {
                    font-size: 12px;
                    color: inherit;
                    text-transform: uppercase;
                }

                
            }

            .active {
                    color: $main_color;
                    box-shadow: inset 0 -3px $main_color;
                }
        }
    }
    
}

</style>