<template>
    <div>
        <header class="d-flex align-items-center">
            <div class="my-container">
                <div class="row justify-content-between my-text-lightgrey align-items-center">

                    <!-- orari di apertura -->
                    <div class="col-6">
                        <i class="fas fa-clock"></i>
                        <span> Open Hours: Mon - sat - 9.00 - 18.00</span>
                    </div>

                    <!-- contatti disponibili -->
                    <div class="col-6">
                        <ul class="d-flex justify-content-between">
                            <li v-for="(connection, index) in listHeaderConnections" :key="index">
                                <a :href="connection.link">
                                    <i :class="connection.icon"></i>
                                    <span> {{connection.text}}</span>
                                </a>
                            </li>
                        </ul>
                    </div>

                </div>
            </div>
        </header>
        <HeaderJumbotron/>
    </div>
</template>

<script>
import HeaderJumbotron from './HeaderJumbotron.vue'

export default {
    name: 'indexHeader',
    components:{
        HeaderJumbotron,
    },
    data: function(){
        return{
            listHeaderConnections:[
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
                    icon: 'fab fa-facebook-f',
                    link:'#'
                },
                {
                    icon: 'fab fa-twitter',
                    link:'#'
                },
                {
                    icon: 'fab fa-linkedin-in',
                    link:'#'
                },
            ]
        }
    }
}
</script>

<style  lang="scss" scoped>
    header{
        background-color: #21333e;
        height: 10vh;
    }
</style>