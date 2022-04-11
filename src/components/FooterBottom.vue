<template>
    <div id="footer-bottom" class="py-5 position-relative">
        <div class="my-container">

            <!-- riga della sezione footer bottom -->
            <div class="row row-cols-2">
                <div class="col">
                    <p class="text-center">Enjoy the low price. We are tracking any intention of piracy</p>
                </div>

                <div class="col">
                    <p class="text-center">©2020 NEXGEN is Prodly Powered by <span class="my-text-green">Codinggs</span>.</p>
                </div>
            </div>
        </div>

        <!-- icona freccia su del footer -->
        <div class="text-end arrow-up">
            <a href="#">
                <i class="fas fa-arrow-up"></i>
            </a>
        </div>
    </div>
</template>

<script>
export default {
    name:'indexFooterBottom'
}
</script>

<style lang="scss" >
@import 'src/assets/style.scss';

div#footer-bottom{
    background-color: black;
    .arrow-up{
        position: absolute;
        top: 50%;
        right: 30px;
        transform: translate(0,-50%);
        i{
            background-color: $my-color-shark;
            color: $my-color-woodsmoke;
            border-radius: 50%;
            padding: 10px;
            font-size: 1.5rem;
        }
    }
}
</style>