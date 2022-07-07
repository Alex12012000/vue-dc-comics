<template>
    <section>
        <div class="container">
            <div class="content">
                <ProductCard v-for="product, index in products" :key="index" :details="product"/>
            </div>
            <div class="tag">
                <span>CURRENT SERIES</span>
            </div>
        </div>
    </section>
</template>


<script>
import ProductCard from './ProductCard.vue'
import productInfo from '../assets/dc-comics.json'


export default {
    name: "MainContentSection",
    components: { 
        ProductCard 
    },
    data() {
        return{
            products: productInfo
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../style/common.scss";
@import "../style/variables.scss";

section {
    background-color: #1c1c1c;
    position: relative;
    .content {
        display: flex;
        justify-content: space-between;
        flex-wrap: wrap;
        padding: 40px;
        color: white;
        
    }

    .tag {
        padding: 8px 20px;
        background-color: $main_color;
        color: white;
        font-size: 23px;
        position: absolute;
        top: -25px;
        left: 150px;
    }
}
</style>