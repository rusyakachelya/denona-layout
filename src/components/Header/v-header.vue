<template>
    <div class="v-header">
        <v-header-top/>
        <v-header-body/>
    </div>
</template>

<script>
import vHeaderTop from  '@/components/Header/v-headerTop.vue'
import vHeaderBody from '@/components/Header/v-headerBody.vue'
// import BgLogo from '@/assets/images/bg-logo.png'

export default {
    name: 'vHeader',
    components: {
        vHeaderTop,
        vHeaderBody,
    },
    props: {

    },
    
}
</script>

<style >
    .v-header{
        height: 100vh;
        background-image: url('@/assets/images/bg-logo.png');
        background-repeat: no-repeat;
        background-size: 1250px;
        background-position: right;
    }
</style>