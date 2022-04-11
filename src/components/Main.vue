<template>
    <main>
        <MainInfoSection/>
        <MainCompanySection/>
        <MainServicesSection/>
        <MainPricingSection/>
        <MainNewsSection/>
        <MainSubscribeSection/>
        <MainSendMessageSection/>
    </main>
</template>

<script>
import MainInfoSection from './MainInfoSection.vue'
import MainCompanySection from './MainCompanySection.vue'
import MainServicesSection from './MainServicesSection.vue'
import MainPricingSection from './MainPricingSection.vue.vue'
import MainNewsSection from './MainNewsSection.vue'
import MainSubscribeSection from './MainSubscribeSection.vue'
import MainSendMessageSection from './MainSendMessageSection.vue'


export default {
    name: 'indexMain',
    components:{
        MainInfoSection,
        MainCompanySection,
        MainServicesSection,
        MainPricingSection,
        MainNewsSection,
        MainSubscribeSection,
        MainSendMessageSection
    }
}
</script>

<style lang="scss">
@import 'src/assets/style.scss';

i{
    color: $my-color-blue-lagoon;
}
</style>