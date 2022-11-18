<template>
    <div class="v-about">
        <div class="container">
                <div class="about__content">
                    <h3 class="about__title">Про NATASHA DENONA</h3>
                    <p class="about__descr">НАТАША, ЯКА ПРОФЕСІЙНИЙ МАЙСТЕР З ПІГМЕНТУ, ОСОБИСТО РОЗРОБЛЯЄ КОЖЕН ПРОДУКТ У ПРОВІДНИХ ІТАЛІЙСЬКИХ ЛАБОРАТОРІЯХ ЗА ВИКОРИСТАННЯМ УДОСКОНАЛЕННОЇ ХУДОЖНЬОЇ ТЕХНІКИ, ЯКУ НЕМОЖЛИВО ТИПІКУВАТИ.</p>
                   <a class="about__link" href="">Читати більше</a>
                </div>
        </div>
    </div>
</template>

<script>

export default {
    name: 'vAbout',
    components: {
       
    },
    props: {
    
    },
    
}
</script>

<style >
   
    .about__title{
        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 500;
        font-size: 32px;
        line-height: 39px;
        color: #EC008C;
        margin-bottom: 20px;
        position: relative;
        margin-left: 80px;
        padding-top: 30px;
        margin-bottom: 50px;
    }
    .about__descr{
        max-width: 500px;
        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 500;
        font-size: 32px;
        line-height: 39px;
        text-align: center;
        color: white;
    }
    .about__content{
        background-image: url('@/assets/images/about.png');
        background-repeat: no-repeat;
        background-position: right;
        height: 600px;
    }
    .about__link{
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
        margin-left: 120px;
    }
</style>