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
    <main class="p-4 text-light">
        <div class="container">
            
            <div class="row row-cols-lg-6 row-cols-md-4 row-cols-sm-3 row-cols-2 gx-0">
                <AppCard v-for="comic, index in comics" :key="index" :pathImage="comic.thumb" :title="comic.series" />
                <!-- <div class="col p-2" v-for="comic, index in comics" :key="index">
                    <img :src="comic.thumb" alt="" class="comicCover">
                    <p class="comicTitle mb-3 text-uppercase">{{ comic.series }}</p>
                </div> -->
            </div>
        </div>
    </main>
</template>
<style lang="scss" scoped>
    main{
        background-color: #1C1C1C;
    }
    
</style>