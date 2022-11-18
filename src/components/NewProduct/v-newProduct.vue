<template>
    <div class="v-new__product">
        <div class="container">
            <div class="new__products">
                <h3 class="new__prod-title">Новинки</h3>
                <div class="new__prod-items">
                    <v-new-product-item
                    v-for="product in newProducts"
                    :key="product.id"
                    :newProducts="product"
                    />
                </div>
               <div class="product__buy"><a class="product__link" href="">Купити онлайн</a></div>
            </div>
        </div>
    </div>
</template>

<script>
import vNewProductItem from '@/components/NewProduct/v-newProductItem.vue'


export default {
    name: 'vNewProduct',
    components: {
       vNewProductItem,
    },
    props: {
        newProducts: {
            type: Array,
            require: true,
        }
    },
    
}
</script>

<style scoped>
    .new__prod-title{
        margin-top: 130px;
        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 500;
        font-size: 36px;
        line-height: 44px;
        color: #EC008C;
        text-align: center;
    }
    .new__prod-items{
        display: flex;
        justify-content: space-around;
    }
    .product__link{
        display: inline-block;
        border: 3px solid #EC008C;
        padding: 16px 19px;
        color: #EC008C;
        font-family: 'Roboto';
        font-style: normal;
        font-weight: 700;
        font-size: 18px;
        line-height: 21px;
        margin-top: 40px;
    }
    .product__buy{
        max-width: 170px;
        margin: 0 auto;
    }
</style>