<script>
export default {
    data(){
        return{
            // definisco un array di oggetti per rendere più modulare la navbar
            links:[
                {
                    label: 'CHARACTERS',
                    url: '#',
                    current: false,
                },
                {
                    label: 'COMICS',
                    url: '#',
                    current: true,
                },
                {
                    label: 'MOVIES',
                    url: '#',
                    current: false,
                },
                {
                    label: 'TV',
                    url: '#',
                    current: false,
                },
                {
                    label: 'GAMES',
                    url: '#',
                    current: false,
                },
                {
                    label: 'COLLECTIBLES',
                    url: '#',
                    current: false,
                },
                {
                    label: 'VIDEOS',
                    url: '#',
                    current: false,
                },
                {
                    label: 'FANS',
                    url: '#',
                    current: false,
                },
                {
                    label: 'NEWS',
                    url: '#',
                    current: false,
                },
                {
                    label: 'SHOP',
                    url: '#',
                    current: false,
                },
            ]
        }
    }
}
</script>
<template>
    <!-- definisco l'header -->
    <header>
        <div class="container">
            <div class="row p-2 justify-content-between align-items-center">
                <div class="col-3 d-flex align-items-center">
                    <!-- aggiungo il logo -->
                    <a href="#"><img src="/dc-logo.png" alt="Logo" class="img-fluid"></a>
                </div>
                <div class="col-9 d-flex align-items-center h-100">
                    <!-- aggiungo la lista per la navbar -->
                    <ul class="list-unstyled d-flex mb-0">
                        <li v-for="(link, index) in links" :key="index" class="ms-3">
                            <a :href="link.url" :class="link.current ? 'active' : ''">{{ link.label }}</a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </header>
</template>
<style lang="scss" scoped> 
header{
    height: 75px;
}
img{
    width: 50px;
}
li{
    font-size: 0.6rem;
    font-weight: 600;
    margin: 0 10px;
    a{
        text-decoration: none;
        color: #000;
        transition: all 0.25s;
    }
    a:hover{
        color: #78aad9;
    }
}
.active{
    color: #0081F8;
    padding: 32px 0;
    border-bottom: 4px solid #0081F8;
}
</style>