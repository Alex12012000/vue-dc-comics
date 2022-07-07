<template>
    <section>
        <div class="container">
            <div class="content">
                <ProductCard v-for="product, index in products" :key="index" :details="product"/>
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

section {
    background-color: #1c1c1c;
    .content {
        display: flex;
        justify-content: space-between;
        align-items: center;
        flex-wrap: wrap;
        padding: 30px;
        color: white;
    }
}
</style>