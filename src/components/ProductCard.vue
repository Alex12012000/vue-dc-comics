<template>
    <div class="card">
        <div class="product-image">
            <img :src="details.thumb" :alt="details.type" >
        </div>

        <div class="text">
            <span>{{details.series}}</span>
        </div>
    </div>
</template>


<script>
export default {
    name: "ProductCard",
    props: {
        details: Object
    }
}
</script>


<style lang="scss" scoped>


.card {
    width: calc((100% / 6) - 20px);
    margin-top: 10px;
    .product-image{
        height: 200px;
        overflow: hidden;
        img {
            height: 100%;
        }
    }

    .text {
        margin: 10px 0;
    }
}


</style>