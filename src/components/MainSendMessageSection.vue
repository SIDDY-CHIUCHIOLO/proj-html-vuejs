<template>
    <section>
        <div class="my-container">
            
            <!-- riga della sezione send a message -->
            <div class="row">
                <!-- colonna con gli input e titolo-->
                <div class="col-8">

                    <!-- titolo -->
                    <span class="my-title-span-green">SEND A MESSAGE</span>
                    <h1 class="my-4 text-dark">Get in<span class="my-bg-opacity-green my-text-green p-2 ms-1">Touch</span></h1>
                    <p class="mb-4">We will responsed to your message as soon as possible.</p>

                    <!-- input -->
                    <div class="w-100 d-flex mb-2">
                        <input class="w-50 me-2" type="text" placeholder="Name">
                        <input class="w-50" type="text" placeholder="Email">
                    </div>
                    <div class="w-100 d-flex mb-2">
                        <input class="w-50 me-2" type="text" placeholder="Phone">
                        <select class="w-50" name="more" id="more-info">
                            <option value="1">More Info</option>
                        </select>
                    </div>
                    <textarea class="w-100 mb-4" type="text" placeholder="Message" rows="5"></textarea>
                    <div>
                        <button class="my-bg-green text-white">SEND</button>
                    </div>
                </div>

                <!-- colonna con exemple inc -->
                <div class="col-4 ps-4">
                    <h5 class="text-dark">Example Inc:</h5>
                    <p class="my-4">Lorem ipsum dolor, sit amet consectetur adipisicing elit.</p>
                    <p class="mb-4">Lorem ipsum dolor, sit amet consectetur adipisicing elit.</p>
                    <ul>
                        <li v-for="(connection, index) in listMainConnections" :key="index">
                            <a :href="connection.link">
                                <i class="my-icon-green mb-4" :class="connection.icon"></i>
                                <span class="my-text-green"> {{connection.text}}</span>
                            </a>
                        </li>
                    </ul>
                    <button class="bg-transparent my-text-green">VIEW MAP</button>
                </div>

            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'indexMainSendMessageSection',
    data: function(){
        return{
            listMainConnections:[
                {
                    icon: 'fas fa-phone-alt',
                    text: '+1(305) 1234-5678',
                    link:'#'
                },
                {
                    icon: 'fas fa-envelope',
                    text: 'hello@example.com',
                    link:'#'
                },
                {
                    icon: 'fas fa-map-marked-alt',
                    text: 'Main Avenue, 987',
                    link:'#'
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import 'src/assets/style.scss';

    section{
        input, textarea, select {
            background-color: $my-color-lightgrey;
        }
    }
</style>