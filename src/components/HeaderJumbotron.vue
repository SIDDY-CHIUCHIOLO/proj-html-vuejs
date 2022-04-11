<template>
<div id="my-header-jumbotron">
    <!-- opacity -->
    <div class="my-opacity-container my-full-height w-100">
        <div class="my-container my-full-height position-relative">

            <!-- navbar con i link -->
            <div class="row text-white">
                <div class="col-12">
                    <nav class="mt-4 d-flex justify-content-between">
                        <img class="my-full-height" src="../assets/img/logo.svg" alt="logo nexgen"> 
                        <ul class="d-flex align-items-center">
                            <li v-for="(element, index) in listHeaderNavLink" :key="index" class="me-4">
                                <a :href="element.link">
                                    <span>{{element.text}}</span>
                                </a>
                            </li>
                            <button class="my-bg-green text-white">GET IN TOUCH</button>
                        </ul>
                    </nav>
                </div>
            </div>

            <!-- titolo del jumbotron -->
            <div class="row text-center text-white title-jumbotron d-flex justify-content-center w-100">
                <div class="col-7">
                    <h1 class="fw-bold mb-4">Lead ~ <span class="my-bg-opacity-green p-2">Customer</span></h1>
                    <p class="mb-4 my-text-lightgrey">Successful strategies require data analysis, creativity and customer focus, taking advantage of the latest technologies to offer excellent services.</p>
                    <button class="my-bg-green me-4 text-white">GET IN TOUCH</button>
                    <button class="bg-transparent text-white">READ MORE</button>
                </div>
            </div>
            
        </div>
    </div>
</div>
</template>

<script>
export default {
    name:'indexHeaderJumbotron',
        data: function(){
        return{
            listHeaderNavLink:[
                {
                    text: 'HOME',
                    link:'#'
                },
                {
                    text: 'ABOUT',
                    link:'#'
                },
                {
                    text: 'SERVICES',
                    link:'#'
                },
                {
                    text: 'PRICING',
                    link:'#'
                },
                {
                    text: 'BLOG',
                    link:'#'
                },
            ]
        }
    }
}
</script>

<style  lang="scss" scoped>
@import 'src/assets/style.scss';

    #my-header-jumbotron{
        background-image: url('../assets/img/hero-image.png');
        background-size: cover;
        background-repeat: no-repeat;
        background-position: center;
        height: 90vh;
        div{
            div.row{
                nav{
                    height: 8vh;
                }
            }
            div.row.title-jumbotron{
                position: absolute;
                top: 50%;
                left: 50%;
                transform: translate(-50%, -50%);
            }
            button.my-bg-green:hover{
                transition: background-color, border;
                transition-duration: 0.5s;
                border:  $my-color-green-hover solid 2px;
                border-radius: 0.25rem;
                background-color:$my-color-green-hover;
            }
        }
    }
</style>