<template>
    <div class="v-header__top">
        <div class="container">
            <div class="header-content">
               <a class="header__logo" href=""><img :src="headerLogo" alt=""></a>
                <ul class="header__list">
                    <li class="header__list-item"><a class="list__item-link" href="">Новинки</a></li>
                    <li class="header__list-item"><a class="list__item-link" href="">Знижки</a></li>
                    <li class="header__list-item"><a class="list__item-link" href="">Обличчя</a></li>
                    <li class="header__list-item"><a class="list__item-link" href="">Очі</a></li>
                    <li class="header__list-item"><a class="list__item-link" href="">Губи</a></li>
                    <li class="header__list-item"><a class="list__item-link" href="">Відгуки</a></li>
                </ul>
                <a class="header__search" href=""><img  :src="headerSearch" alt=""></a>
            </div>
        </div>
    </div>
</template>

<script>
import header__search from '@/assets/images/header-search.png'
import header__logo from '@/assets/images/header-logo.png'

export default {
    name: 'vHeaderTop',
    computed: {
        headerSearch() {
            return header__search
        },
        headerLogo() {
            return header__logo
        }
    }
}
</script>

<style>
    .v-header__top{
       color: wheat;
       padding: 15px 0;
    }
    .header-content{
        display: flex;
        justify-content: flex-start;
        align-items: center;
    }
    .header__list{
        display: flex;
        list-style:  none;
        margin-left: 50px;
    }
    .header__list-item{
        margin-right: 25px;
        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 400;
        font-size: 18px;
        line-height: 22px;
    }
    .header__list-item:last-child{
        margin-right: 0;
    }
    .header__search{
        margin-left: 150px;
    }
    a{
        text-decoration: none;
        color: white;
    }
</style>