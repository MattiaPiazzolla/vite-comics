<script>
export default {
    data(){
        return{
           bannerElements:[
            {
                icon:'/public/buy-comics-digital-comics.png',
                text: 'DIGITAL COMICS',
                url:'#'
            },
            {
                icon:'/public/buy-comics-merchandise.png',
                text: 'DC MERCHANDISE',
                url:'#'
            },
            {
                icon:'/public/buy-comics-subscriptions.png',
                text: 'SUBSCRIPTION',
                url:'#'
            },
            {
                icon:'/public/buy-comics-shop-locator.png',
                text: 'COMIC SHOP LOCATOR',
                url:'#'
            },
            {
                icon:'/public/buy-dc-power-visa.svg',
                text: 'DC POWER VISA',
                url:'#'
            },
           ] 
        }
    }
}
</script>
<template>
    <div class="banner d-flex align-items-center justify-content-center">
        <div class="container text-center">
            <ul class="list-unstyled d-flex justify-content-center m-0 p-0">
                <li v-for="(elem, index) in bannerElements" :key="index" class="text-light d-flex justify-content-center align-items-center me-5">
                    <a :href="elem.url" class="text-decoration-none d-flex align-items-center">
                        <img :src="elem.icon" class="me-2" :alt="elem.text">
                        {{ elem.text }}
                    </a>
                </li>
            </ul>
        </div>
    </div>
</template>
<style lang="scss" scoped>
    .banner{
        background-color: #0081F8;
        height: 100px;
        overflow: hidden;
    }

    li{
        color: #fff;
        font-size: 0.6rem;
        font-weight: 400;
        width: 100%;
        img{
            //chiedi come gestire l'svg
            width: 27.5px;
            transition: all 0.25s;
        }
        a{
            text-decoration: none;
            color: #fff;
            transition: all 0.25s;
        }
        a:hover{
            color: #000000;
        }
        a:hover img{
            filter: brightness(0);
        }
        
    }

</style>