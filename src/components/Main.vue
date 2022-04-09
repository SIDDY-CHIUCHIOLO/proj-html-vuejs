<template>
    <div>
        <MainInfoSection/>
        <MainCompanySection/>
        <MainServicesSection/>
        <MainPricingSection/>
        <MainNewsSection/>
    </div>
</template>

<script>
import MainInfoSection from './MainInfoSection.vue'
import MainCompanySection from './MainCompanySection.vue'
import MainServicesSection from './MainServicesSection.vue'
import MainPricingSection from './MainPricingSection.vue.vue'
import MainNewsSection from './MainNewsSection.vue'




export default {
    name: 'indexMain',
    components:{
        MainInfoSection,
        MainCompanySection,
        MainServicesSection,
        MainPricingSection,
        MainNewsSection
    }
}
</script>

<style lang="scss" >
@import 'src/assets/style.scss';
</style>