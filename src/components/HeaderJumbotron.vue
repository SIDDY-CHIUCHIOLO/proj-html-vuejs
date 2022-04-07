<template>
<div id="my-header-jumbotron" class="my-height">
    <div class="my-opacity-container my-height w-100">
        <div class="my-container">
            <div class="row text-white">
                <div class="col-12">

                    <!-- navbar con i link -->
                    <nav class="my-4 d-flex justify-content-between">
                        <h5 class="fw-bold"><span class="my-bg-text-green">N E X</span> G E N</h5>
                        <ul class="d-flex align-items-center">
                            <li v-for="(element, index) in listHeaderNavLink" :key="index" class="me-4">
                                <a :href="element.link">
                                    <span>{{element.text}}</span>
                                </a>
                            </li>
                            <button class="btn text-white py-2 px-3">GET IN TOUCH</button>
                        </ul>
                    </nav>

                </div>
            </div>
            <div class="row text-center text-white d-flex justify-content-center">
                <div class="col-7">
                    <h1 class="fw-bold">Lead ~ Customer</h1>
                    <p>successful strategies require data analysis, creativity and customer focus, taking advantage of the latest technologies to offer excellent services.</p>
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
        background-image: url('@/assets/img/hero-image.png');
        background-size: cover;
        background-repeat: no-repeat;
        background-position: center;
        div.my-opacity-container{
            background-color: rgba(0, 0, 0, 0.7) ;
            h5{
                span{
                    border-radius: 50px 0 0 50px;
                    padding: 13px 3px 13px 40px;
                }
            }
            ul{
                button{
                    background-color: #058283;
                }
            }
        }
    }
</style>