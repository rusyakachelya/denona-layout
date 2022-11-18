<template>
    <div class="v-header__body">
        <div class="container">
            <div class="body__content">
                <h1 class="body__title">
                    MY DREAM COLLECTION
                </h1>
                <p class="body__descr">
                    Нові яскраві палетки в новій коллекції
                </p>
                <a class="body__link" href="">Дізнатись більше про новинки</a>
            </div>
        </div>
    </div>
</template>

<script>

export default {
    name: 'vHeaderBody',
    components: {
       
    },
    props: {

    },
    
}
</script>

<style >
    .v-header__body{
        margin-top: 180px;
    }
    .body__title{
        max-width: 400px;
        text-transform: uppercase;
        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 800;
        font-size: 64px;
        line-height: 78px;
        color: purple;
    }
    .body__descr{
        margin-top: 35px;
        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 400;
        font-size: 24px;
        line-height: 29px;
        color: white;
        max-width: 350px;
        padding-bottom: 42px;
    }
    .body__link{
        display: inline-block;
        margin-top: 40px;
        padding: 16px 19px;
        color: #EC008C;
        border: 3px solid #EC008C;
    }
</style>