<template>
    <section class="d-flex align-items-center">
        <div class="my-container">
            <div class="row row-cols-3">

                <div class="col">
                    <div class="my-card bg-white">
                        <i class="fas fa-user-friends"></i>
                        <h5 class="card-title fw-bold mb-3 text-dark">Human Capital</h5>
                        <p class="card-text">Humanizing business: Hearness the power of technology to improve the way people work.</p>
                    </div>
                </div>

                <div class="col">
                    <div class="my-card bg-white">
                        <i class="fas fa-chart-pie"></i>
                        <h5 class="card-title fw-bold mb-3 text-dark">Core Business</h5>
                        <p class="card-text">It takes innovative approaches to taransform, modernize, and run existing platform.</p>
                    </div>
                </div>

                <div class="col">
                    <div class="my-card bg-white">
                        <i class="fas fa-tachometer-alt"></i>
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
    name:'indexMainSectionInfo'
}
</script>

<style  lang="scss" scoped>
@import 'src/assets/style.scss';

section{
    background-color: $my-color-gray-nurse;
    height: 50vh;
    width: 100%;
    i{
        color: $my-color-blue-lagoon;
        background-color: $my-color-gray-nurse;
        border-radius: 50%;
        padding: 12px 10px;
        margin-bottom: 1rem;
        font-size: 1.5rem;
    }
}
</style>