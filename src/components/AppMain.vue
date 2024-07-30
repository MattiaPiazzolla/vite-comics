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
            
            <AppCard />

            <ul>
                <li v-for="comic, index in comics" :key="index">
                    <img :src="comic.thumb" alt="">
                </li>
            </ul>
        </div>
    </main>
</template>
<style lang="scss">
    main{
        background-color: #1C1C1C;
    }
</style>