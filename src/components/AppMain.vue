<script>
import AppCard from './partials/AppCard.vue';

export default {
    components:{
        AppCard,
    },
    
}
</script>
<template>
    <main class="p-4 text-light">
        <div class="container">
            
            <AppCard />
        </div>
    </main>
</template>
<style lang="scss">
    main{
        background-color: #1C1C1C;
    }
</style>