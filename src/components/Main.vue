<template>
    <div>
        <MainSectionInfo/>
        <MainSectionCompany/>
    </div>
</template>

<script>
import MainSectionInfo from './MainSectionInfo.vue'
import MainSectionCompany from './MainSectionCompany.vue'


export default {
    name: 'indexMain',
    components:{
        MainSectionInfo,
        MainSectionCompany
    }
}
</script>

<style lang="scss" >
@import 'src/assets/style.scss';
</style>