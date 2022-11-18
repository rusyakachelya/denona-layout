<template>
    <div class="v-footer">
        <div class="container">
            <div class="footer__lists">

                <div class="products">
                    <h6 class="product__name">Продукти</h6>
                    <ul class="products__links">
                        <li class="product__item"><a class="product__link" href="">Новинки</a></li>
                        <li class="product__item"><a class="product__link" href="">Обличчя</a></li>
                        <li class="product__item"><a class="product__link" href="">Очі</a></li>
                        <li class="product__item"><a class="product__link" href="">Губи</a></li>
                    </ul>
                </div>  

                 <div class="products">
                    <h6 class="product__name">Історія бренду</h6>
                    <ul class="products__links">
                        <li class="product__item"><a class="product__link" href="">История NATASHA DENONA</a></li>
                        <li class="product__item"><a class="product__link" href="">Поради новачкам</a></li>
                        <li class="product__item"><a class="product__link" href="">Ідеї для макіяжа</a></li>
                        <li class="product__item"><a class="product__link" href="">Наші клієнти</a></li>
                    </ul>
                </div>

                 <div class="products">
                    <h6 class="product__name">Юридична інформація</h6>
                    <ul class="products__links">
                        <li class="product__item"><a class="product__link" href="">Контакти</a></li>
                        <li class="product__item"><a class="product__link" href="">Конфиденційність</a></li>
                        <li class="product__item"><a class="product__link" href="">Очі</a></li>
                    </ul>
                </div>

              
            </div>
            <p class="footer__text">California Transparency In Supply Chains Act 2022</p>
        </div>
    </div>
</template>

<script>
export default {
    name: 'vFooter',
}
</script>

<style scoped>
    .v-footer{
        border: 1px solid #FFFFFF;
        color: white;
        padding-bottom: 30px;
    }
    .footer__lists{
        padding-top: 80px;
        display: flex;
        justify-content: space-between;
 
    }
    .product__name{
        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 400;
        font-size: 24px;
        line-height: 29px;
        text-align: center;
        margin-bottom: 55px;
    }
    .product__item{
        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 400;
        font-size: 16px;
        line-height: 20px;
        margin-bottom: 35px;
    }
    .footer__text{
        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 400;
        font-size: 16px;
        line-height: 20px;
        color: rgba(255, 255, 255, 0.55);
        text-align: end;
    }
</style>