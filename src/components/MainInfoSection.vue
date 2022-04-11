<template>
    <section class="d-flex">
        <div class="my-container">
            <div class="row row-cols-3">

                <div class="col">
                    <div class="my-card bg-white">
                        <i class="fas fa-user-friends my-icon-green"></i>
                        <h5 class="card-title mb-3 text-dark">Human Capital</h5>
                        <p class="card-text">Humanizing business: Hearness the power of technology to improve the way people work.</p>
                    </div>
                </div>

                <div class="col">
                    <div class="my-card bg-white">
                        <i class="fas fa-chart-pie my-icon-green"></i>
                        <h5 class="card-title mb-3 text-dark">Core Business</h5>
                        <p class="card-text">It takes innovative approaches to taransform, modernize, and run existing platform.</p>
                    </div>
                </div>

                <div class="col">
                    <div class="my-card bg-white">
                        <i class="fas fa-tachometer-alt my-icon-green"></i>
                        <h5 class="card-title fw-bold mb-3 text-dark">Performance</h5>
                        <p class="card-text">Archieving maximum impact and value from investments in finance and supply chain.</p>
                    </div>
                </div>

            </div>
        </div>
    </section>
</template>

<script>

export default {
    name:'indexMainInfoSection'
}
</script>

<style  lang="scss" scoped>
@import 'src/assets/style.scss';

section{
    background-color: $my-color-gray-nurse;
    width: 100%;
}
</style>