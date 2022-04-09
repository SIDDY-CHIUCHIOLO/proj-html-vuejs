<template>
    <section class="py-5">
        <div class="my-container">

            <!-- titolo della sezione -->
            <div class="row">
                <div class="col-12">
                    <span class="my-title-span-green">OUR EDITORIAL CONTENT</span>
                    <h1 class="my-4 text-dark">Latest <span class="my-bg-opacity-green my-text-green p-2 me-1">News</span></h1>
                </div>
                <div class="d-flex align-items-center justify-content-between mb-5">
                    <p>Every week publish content about what is best in the business world</p>
                    <button class="my-bg-green text-white">SEE ALL</button>
                </div>
            </div>

            <!-- cards della sezione -->
            <div class="row row-cols-3">
                <!-- card left -->
                <div class="col">
                    <div class="my-card card-left bg-dark position-relative">
                        <div class="my-opacity-container">
                            <h5 class=" text-white text-center m-5">Increasing creativity is possible for everyone</h5>
                        </div>
                    </div>
                </div>

                <!-- card center-->
                <div class="col">
                    <div class="my-card card-center bg-dark position-relative">
                        <div class="my-opacity-container">
                            <h5 class=" text-white text-center m-5">Because market research is part of the business plan</h5>
                        </div>
                    </div>
                </div>
                
                <!-- card right -->
                <div class="col">
                    <div class="my-card card-right bg-dark position-relative">
                        <div class="my-opacity-container">
                            <h5 class=" text-white text-center m-5">Working from home is now a trend</h5>
                        </div>
                    </div>
                </div>
            </div>
            
        </div>
    </section>
</template>

<script>
export default {
    name: 'indexMainNewsSection'
}
</script>

<style  lang="scss" scoped>
@import 'src/assets/style.scss';

    section{
        .my-card{
            height: 313.15px;
            background-size: cover;
            background-repeat: no-repeat;
            background-position: center;
            .my-opacity-container{
                height: 100%;
                width: 100%;
                position: absolute;
                top: 0;
                left: 0;
                border-radius: 0.5rem;
                display: flex;
                flex-direction: column;
                justify-content: end;
            }
        }
        .card-left{
            background-image: url('../assets/img/news-1.jpg');
        }
        .card-center{
            background-image: url('../assets/img/news-2.jpg');
        }
        .card-right{
            background-image: url('../assets/img/news-3.jpg');
        }
    }
</style>