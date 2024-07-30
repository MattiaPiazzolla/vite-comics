<script>
export default {
    props:{
        pathImage: String,
        title: String,
        price: String,
        type: String
    }
}
</script>

<template>
    <div class="col p-2">
        <img :src="pathImage" :alt="title" class="comicCover">
        <p class="comicTitle mb-3 text-uppercase">{{ title }}</p>
    </div>
</template>

<style lang="scss" scoped>
    .comicTitle{
        font-size: 0.7rem;
        margin-top: 10px;   
    }
</style>