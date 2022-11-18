<template>
    <div class="v-advice">
        <div class="container">
            <div class="advice">
                <h3 class="advice__title">Поради по нанесенню макіяжу</h3>
                <div class="advice__box">
                    <img class="advice__img" src="@/assets/images/model.png" alt="">
                    <ul class="advice__list">
                        <li class="advice__item-one">Щоб підібрати відповідний відтінок <br>тональної основи, нанеси її на лінію<br> підборіддя</li>
                        <li class="advice__item-two">Для більш щільного покриття наноси<br> тональну основу спонжем, для<br> легшого – пензлем.</li>
                        <li class="advice__item-three">Приховуйте будь-які дефекти шкіри<br> протягом дня, наносячи основу<br> пальцями або пензлем для<br> консилера.</li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</template>

<script>


export default {
    name: 'vAdvice',

}
</script>

<style>
    .v-advice{
        padding-bottom: 120px;
    }
    .advice__title{
        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 500;
        font-size: 36px;
        line-height: 44px;
        color: #EC008C;
        margin-top: 124px;
        text-align: center;
        margin-bottom: 41px;
    }
    .advice__box{
        display: flex;
        justify-content: space-between;
    }
    .advice__list{
        width: 466px;
    }
    .advice__item-one::after{
        content: url('@/assets/images/adviceOne.png');
        position: absolute;
            left: -80px;
    top: -10px;
    }
    .advice__item-two::after{
        content: url('@/assets/images/adviceTwo.png');
        position: absolute;
            left: -80px;
    top: -10px;
    }
    .advice__item-three::after{
        content: url('@/assets/images/adviceThree.png');
        position: absolute;
            left: -80px;
    top: -10px;
    }
     .advice__item-one{
        position: relative;
     }
      .advice__item-two{
        position: relative;
    }
     .advice__item-three{
        position: relative;
     }
    ul{
        margin-top: 60px;
        list-style: none;
        color: white;
    }
    .advice__list li{
        margin-bottom: 80px;
    }
</style>