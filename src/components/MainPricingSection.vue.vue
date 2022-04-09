<template>
    <section class="py-5">
        <div class="my-container">
            <!-- titolo della sezione -->
            <div class="row text-center justify-content-center">
                <div class="col-8">
                    <span class="my-title-span-green">MONTHLY PLANS</span>
                    <h1 class="my-4 text-dark"><span class="my-bg-opacity-green my-text-green p-2 me-1">Pricing</span>Table</h1>
                    <p class="mb-5">We can help deliver and  excute your future, wherever you complete, using the latest technologies, from strategy development to implementation.</p>
                </div>
            </div>
            <div class="row row-cols-3 align-items-center">

                <!-- offerta standard -->
                <div class="col">
                    <div class="my-card bg-white text-center">
                        <i class="fas fa-rocket fs-1"></i>
                        <h5 class="card-title mb-3 text-dark">Standard</h5>
                        <p class="card-text mb-3 my-text-green fw-bold">$ <span class="fs-1">490</span> /mo</p>
                        <ul>
                            <li class="d-flex justify-content-between pb-2" v-for='(offer, index) in listOfOfferStandard' :key="index">
                                <p>{{offer.text}}</p>
                                <i class="fs-6" :class="offer.icon"></i>
                            </li>
                        </ul>
                    </div>
                </div>

                <!-- offerta professional -->
                <div class="col">
                    <div class="my-card bg-white text-center position-relative py-5">

                        <!-- offerta più popolare -->
                        <div class="most-popular-offer">
                            <p>Most</p>
                            <p>Popular</p>
                        </div>
                        <i class="fas fa-briefcase fs-1"></i>
                        <h5 class="card-title mb-3 text-dark">Professional</h5>
                        <p class="card-text mb-3 my-text-green fw-bold">$ <span class="fs-1">890</span> /mo</p>
                        <ul>
                            <li class="d-flex justify-content-between pb-2" v-for='(offer, index) in listOfOfferProfessional' :key="index">
                                <p>{{offer.text}}</p>
                                <i class="fs-6" :class="offer.icon"></i>
                            </li>
                        </ul>
                    </div>
                </div>

                
                <!-- offerta ultimate -->
                <div class="col">
                    <div class="my-card bg-white text-center">
                        <i class="far fa-gem fs-1"></i>
                        <h5 class="card-title mb-3 text-dark">Ultimate</h5>
                        <p class="card-text mb-3 my-text-green fw-bold">$ <span class="fs-1">1.390</span> /mo</p>
                        <ul>
                            <li class="d-flex justify-content-between pb-2" v-for='(offer, index) in listOfOfferUltimate' :key="index">
                                <p>{{offer.text}}</p>
                                <i class="fs-6" :class="offer.icon"></i>
                            </li>
                        </ul>
                    </div>
                </div>

            </div>
        </div>
    </section>
</template>

<script>
export default {
    name:'indexMainPricingSection.vue',
    data: function(){
        return{
            listOfOfferStandard:[
                {
                    text: 'Standard Accounting',
                    icon:'fa fa-check'
                },
                {
                    text: 'Platform Access',
                    icon:'fas fa-check'
                },
                {
                    text: 'Business Orientation',
                    icon:'fas fa-times'
                },
                {
                    text: 'Dedicated Consultant',
                    icon:'fas fa-times'
                },
                {
                    text: 'Personal Assistance',
                    icon:'fas fa-times'
                },
            ],
            listOfOfferProfessional:[
                {
                    text: 'Standard Accounting',
                    icon:'fa fa-check'
                },
                {
                    text: 'Platform Access',
                    icon:'fas fa-check'
                },
                {
                    text: 'Business Orientation',
                    icon: 'fa fa-check'
                },
                {
                    text: 'Dedicated Consultant',
                    icon:'fas fa-times'
                },
                {
                    text: 'Personal Assistance',
                    icon:'fas fa-times'
                },
            ],
            listOfOfferUltimate:[
                {
                    text: 'Standard Accounting',
                    icon:'fa fa-check'
                },
                {
                    text: 'Platform Access',
                    icon:'fas fa-check'
                },
                {
                    text: 'Business Orientation',
                    icon: 'fa fa-check'
                },
                {
                    text: 'Dedicated Consultant',
                    icon:'fas fa-check'
                },
                {
                    text: 'Personal Assistance',
                    icon:'fas fa-check'
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import 'src/assets/style.scss';

    section{
        background-color: $my-color-gray-nurse;
        .most-popular-offer {
            position: absolute;
            background-color:  $my-color-blue-lagoon;
            border-end-end-radius: 50%;
            border-start-end-radius: 50%;
            top: 0.8rem;
            left: 0;
            font-size: 0.8rem;
            padding: 0.5rem 1.2rem 0.5rem 0.5rem;
            color: white;
            font-weight: bold;
            text-align: left;
        }
    }
</style>