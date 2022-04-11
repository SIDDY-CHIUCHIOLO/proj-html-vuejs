<template>
    <section>
        <div class="my-container">

            <!-- titolo della sezione services-->
            <div class="row">
                <div class="col-12">
                    <span class="my-title-span-green">OUR BUSINESS AREAS</span>
                    <h2 class="text-white my-4">Excellence <span class="my-bg-opacity-green p-2">Services</span></h2>
                </div>
                <div class="col-10">
                    <p class="mb-5">We are leaders in providing consultancy with a set of cutting-edge technologies and a team of experienced and renowned professionals. These are some options that you can hire</p>
                </div>
                <div class="col-2">
                    <button class="bg-transparent text-white">SEE ALL</button>
                </div>
            </div>

            <!-- riga con le card -->
            <div class="row row-cols-3 mb-4">

                <!-- card Audit & Assurance -->
                <div class="col">
                    <div class="my-card">
                        <i class="fas fa-sitemap"></i>
                        <h5 class="card-title mb-3 text-white">Audit & Assurance</h5>
                        <p class="card-text mb-3">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                        <button class="bg-transparent">READ MORE</button>
                    </div>
                </div>

                <!-- card Financial Advisory -->
                <div class="col">
                    <div class="my-card">
                        <i class="fas fa-briefcase"></i>
                        <h5 class="card-title mb-3 text-white">Financial Advisory</h5>
                        <p class="card-text mb-3">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                        <button class="bg-transparent">READ MORE</button>
                    </div>
                </div>

                <!-- card Analytics and M&A -->
                <div class="col">
                    <div class="my-card">
                        <i class="far fa-chart-bar"></i>
                        <h5 class="card-title mb-3 text-white">Analytics and M&A</h5>
                        <p class="card-text mb-3">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                        <button class="bg-transparent">READ MORE</button>
                    </div>
                </div>
            </div>

            <!-- seconda riga con le card -->
            <div class="row row-cols-3">

                <!-- card Middle Marketing -->
                <div class="col">
                    <div class="my-card">
                        <i class="fas fa-plane"></i>
                        <h5 class="card-title mb-3 text-white">Middle Marketing</h5>
                        <p class="card-text mb-3">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                        <button class="bg-transparent">READ MORE</button>
                    </div>
                </div>

                <!-- card Legal Consulting -->
                <div class="col">
                    <div class="my-card">
                        <i class="fas fa-globe"></i>
                        <h5 class="card-title mb-3 text-white">Legal Consulting</h5>
                        <p class="card-text mb-3">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                        <button class="bg-transparent">READ MORE</button>
                    </div>
                </div>
                
                <!-- card Regulatory Risk -->
                <div class="col">
                    <div class="my-card">
                        <i class="fas fa-bars"></i>
                        <h5 class="card-title mb-3 text-white">Regulatory Risk</h5>
                        <p class="card-text mb-3">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                        <button class="bg-transparent">READ MORE</button>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'indexMainServicesSection'
}
</script>

<style lang="scss" scoped>
@import 'src/assets/style.scss';

    section{
        background-color: $my-color-woodsmoke;
        .my-card{
            background-color: $my-color-shark;
            button{
                color: white;
            }
        }
        .my-card:hover{
            transform: translate(-0, -5%);
            transition-duration: 1s;
        }
    }
</style>