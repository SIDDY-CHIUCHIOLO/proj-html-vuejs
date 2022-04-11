<template>
    <section>
        <div class="my-container">
            <div class="row row-cols-2">

                <!-- titolo della sezione -->
                <div class="col">
                    <span class="my-title-span-green">NEWSLETTER</span>
                    <h1 class="my-4 text-white"><span class="my-bg-opacity-green text-white p-2 me-1">Know</span>Fist</h1>
                    <p>Follow closly and receive content about our company and the news of the current market.</p>
                </div>

                <!-- iput della sezione -->
                <div class="col">
                    <div class="d-flex flex-column justify-content-between my-full-height">
                        <input class="w-100" type="text" placeholder="Name">
                        <input class="w-100" type="text" placeholder="Email">
                        <div>
                            <button class="my-bg-green text-white">SUBSCRIBE</button>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'indexMainSubscribeSection'
}
</script>

<style lang="scss" scoped>
@import 'src/assets/style.scss';
    
    section{
        background-size: cover;
        background-repeat: no-repeat;
        background-position: center;
        background-image: url('../assets/img/bg-1.jpg');
        input{
            background-color: $my-color-edward-opacity;
        }
    }
</style>