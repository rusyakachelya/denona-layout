<template>
    <div class="v-new__product-item">
            <div class="product__item">
                <img class="prod__item-img" :src="newProducts.img" alt="">
                <p class="pod__item-title">{{newProducts.title}}</p>
            </div>
    </div>
</template>

<script>

export default {
    name: 'vNewProductItem',
    components: {
       
    },
    props: {
        newProducts: {
            type: Object,
            require: true
        }
    },
    
}
</script>

<style >
    .v-new__product-item{
        margin-top: 70px;
    }
    .prod__item-img{
        margin-bottom: 20px;
    }
    .pod__item-title{
        font-weight: 500;
        font-size: 24px;
        line-height: 29px;
        color: white;
        text-align: center;
        max-width: 240px;
    }
</style>