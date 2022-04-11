<template>
    <header>
        <HeaderTop/>
        <HeaderBottomJumbotron/>
    </header>
</template>

<script>
import HeaderTop from './HeaderTop.vue'
import HeaderBottomJumbotron from './HeaderBottomJumbotron.vue'

export default {
    name: 'indexHeader',
    components:{
        HeaderTop,
        HeaderBottomJumbotron,
    },
}
</script>

<style  lang="scss">
</style>