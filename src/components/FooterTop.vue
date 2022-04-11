<template>
    <section id="footer-top">
        <div class="my-container">
            <div class="row row-cols-4">

                <!-- colonna con i conntatti -->
                <div class="col">
                    <img class="w-50" src="../assets/img/logo.svg" alt="logo nexgen">
                    <p class="my-4">A Functional HTML Template for Corporate & Business.</p>
                    <ul>
                        <li v-for="(connection, index) in listFooterConnections" :key="index">
                            <a :href="connection.link">
                                <i class="mb-4 me-1" :class="connection.icon"></i>
                                <span> {{connection.text}}</span>
                            </a>
                        </li>
                    </ul>
                    <button class="bg-transparent text-white">GET IN TOUCH</button>
                </div>

                <!-- colonna link about -->
                <div class="col">
                    <div class="my-card">
                        <h5 class="card-title mb-3 text-white">About</h5>
                        <ul>
                            <li v-for="(element, index) in listFooterAbout" :key="index">
                                <a :href="element.link">
                                    <i class="fas fa-angle-right me-2"></i>
                                    <span>{{element.text}}</span>
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>

                <!-- colonna link services -->
                <div class="col">
                    <div class="my-card">
                        <h5 class="card-title mb-3 text-white">Services</h5>
                        <ul>
                            <li v-for="(element, index) in listFooterServices" :key="index">
                                <a :href="element.link">
                                    <i class="fas fa-angle-right me-2"></i>
                                    <span>{{element.text}}</span>
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>

                <!-- colonna link support -->
                <div class="col">
                    <div class="my-card">
                        <h5 class="card-title mb-3 text-white">Support</h5>
                        <ul>
                            <li v-for="(element, index) in listFooterSupport" :key="index">
                                <a :href="element.link">
                                    <i class="fas fa-angle-right me-2"></i>
                                    <span>{{element.text}}</span>
                                </a>
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
    name:'indexFooterTop',
    data: function(){
        return{
            listFooterConnections:[
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
            ],
            listFooterAbout:[
                {
                    text:'The company',
                    link:'#'
                },
                {
                    text:'Institutional',
                    link:'#'
                },
                {
                    text:'Social & Events',
                    link:'#'
                },
                {
                    text:'Innovation',
                    link:'#'
                },
                {
                    text:'Enviroment',
                    link:'#'
                },
                {
                    text:'Technology',
                    link:'#'
                },
            ],
            listFooterServices:[
                {
                    text:'Audit & Assurance',
                    link:'#'
                },
                {
                    text:'Financial Advisory',
                    link:'#'
                },
                {
                    text:'Analystick M&A',
                    link:'#'
                },
                {
                    text:'Middle Marketing',
                    link:'#'
                },
                {
                    text:'Legal Consulting',
                    link:'#'
                },
                {
                    text:'Regulatory Risk',
                    link:'#'
                },
            ],
            listFooterSupport:[
                {
                    text:'Responsability',
                    link:'#'
                },
                {
                    text:'Term of Use',
                    link:'#'
                },
                {
                    text:'About Cookies',
                    link:'#'
                },
                {
                    text:'Privacy Plicy',
                    link:'#'
                },
                {
                    text:'Accasibility',
                    link:'#'
                },
                {
                    text:'Information',
                    link:'#'
                },
            ]
        }
    }
}
</script>

<style lang="scss" >
@import 'src/assets/style.scss';

section#footer-top{
    background-color: $my-color-woodsmoke;
    .my-card{
        background-color: $my-color-shark;
        i{
            color: $my-color-edward;
        }
    }
}
</style>