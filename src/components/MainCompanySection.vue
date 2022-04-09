<template>
    <section class="my-height-80vh d-flex position-relative align-items-center">
        <div class="my-container">
            <div class="row w-50">
                <div class="col-12">
                    <span class="my-title-span-green">ABOUT THE NETWORK</span>
                    <h2  class="text-dark my-4"><span class="my-text-green my-bg-grey p-2">The</span>Company</h2>
                    <p class="mb-5">For 12 years we have been providing audit and warranty, financial advice, risk advice, texes related services to select clients</p>
                </div>
            </div>

            <div class="row w-50 row-cols-2 mb-5">
                <div class="col">
                    <i class="fas fa-medal my-text-green"></i>
                    <h5 class="text-dark d-inline">Tradition</h5>
                    <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit.</p>
                </div>

                <div class="col">
                    <i class="fas fa-lock"></i>
                    <h5 class="text-dark d-inline">Security</h5>
                    <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit.</p>
                </div>
            </div>

            <div class="row w-50 row-cols-2">
                <div class="col">
                    <i class="far fa-edit"></i>
                    <h5 class="text-dark d-inline">Certificate</h5>
                    <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit.</p>
                </div>

                <div class="col">
                    <i class="fas fa-brain"></i>
                    <h5 class="text-dark d-inline">Expertise</h5>
                    <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit.</p>
                </div>
            </div>

        </div>
        <div class="w-50 my-full-height contain-img-company position-absolute"></div>
    </section>
</template>

<script>
export default {
    name: 'indexMainCompanySection'
}
</script>

<style  lang="scss" scoped>
@import 'src/assets/style.scss';

    section{
        .contain-img-company{
            background-image: url('../assets/img/about-3.jpg');
            background-position: center;
            background-size: cover;
            background-repeat: no-repeat;
            top: 0;
            right: 0;
        }
        i{
            color: $my-color-blue-lagoon;
            font-size: 1.4rem;
            margin-right: 0.5rem;
            margin-bottom: 1.8rem;
        }
    }
</style>