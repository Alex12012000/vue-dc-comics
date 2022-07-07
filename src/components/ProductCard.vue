<template>
    <div class="card">
        <div class="product-image">
            <img :src="details.thumb" :alt="details.type" >
        </div>
        <span>{{details.series}}</span>
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
    
    .product-image{
        height: 200px;
        overflow: hidden;
        margin: 20px 0;
    }

    span {
        font-size: 15px;
    }
    
}


</style>