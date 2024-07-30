<script>
import AppCard from './partials/AppCard.vue';
import comics from '../data/comics';

export default {
    components:{
        AppCard,
    },
    data() {
        return {
            comics
        }
    },
    
}
</script>
<template>
    <main class="text-light">
        <div class="jumbo">
            <div class="container position-relative h-100">
                <div class="labelSection">CURRENT SERIES</div>
            </div>
        </div>

        <div class="container p-4">
            
            <div class="row row-cols-lg-6 row-cols-md-4 row-cols-sm-3 row-cols-2 gx-0">
                <AppCard v-for="comic, index in comics" :key="index" :pathImage="comic.thumb" :title="comic.series" :price="comic.price"/>
                <!-- <div class="col p-2" v-for="comic, index in comics" :key="index">
                    <img :src="comic.thumb" alt="" class="comicCover">
                    <p class="comicTitle mb-3 text-uppercase">{{ comic.series }}</p>
                </div> -->
            </div>
            <div class="w-100 d-flex justify-content-center mb-0">
                <button class="btnLoad py-2 px-4 text-light">LOAD MORE</button>
            </div>
        </div>
    </main>
</template>
<style lang="scss" scoped>
    main{
        background-color: #1C1C1C;
    }
    .jumbo{
        background-image: url('/public/jumbotron.jpg');
        background-repeat: no-repeat;
        background-size: cover;
        height: 25dvh;
    }

    .btnLoad{
        background-color: #0081F8;
        border: 0;
        font-size: 0.5rem;
        font-weight: 600;
        &:hover{
            background-color: #0167c7;
        }
    }
    .labelSection{
        position: absolute;
        padding: 7.5px;
        background-color: #0081F8;
        border: 0;
        font-size: 0.75rem;
        font-weight: 600; 
        bottom: -5%;
        left: -4%;
        transform: translate(50%);

    }
</style>