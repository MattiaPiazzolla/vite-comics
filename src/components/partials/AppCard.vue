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
    <div class="col p-2 comic position-relative">
        <p class="position-absolute priceComic">{{ price }}</p>
        <img :src="pathImage" :alt="title" class="comicCover">
        <p class="comicTitle mb-3 text-uppercase">{{ title }}</p>
    </div>
</template>

<style lang="scss" scoped>
    .comicTitle{
        font-size: 0.7rem;
        margin-top: 10px;   
    }
    .comic{
        cursor: pointer;
        img{
            transition: all 0.3s;
        }
        .priceComic{
            bottom: 50%;
            left: 50%;
            transform: translateX(-50%);
            opacity: 0;
            font-weight: 700;
            z-index: 100;
            transition: all 0.5s;
        }
        &:hover{
            img{
                filter: brightness(0.25);
                scale: 1.01;
            }
            .priceComic{
                opacity: 1;
            }
        }
    }
    

</style>