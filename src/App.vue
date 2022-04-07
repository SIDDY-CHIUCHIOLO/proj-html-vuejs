<template>
  <div id="app">
    <Header/>
  </div>
</template>

<script>
import Header from './components/Header.vue'

export default {
  name: 'App',
  components: {
    Header,
  }
}
</script>

<style lang="scss">
@import 'src/assets/style.scss';

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  p{
    margin: 0;
  }
  a{
    text-decoration: none;
    color: $my-text-color;
  }
  ul{
    list-style: none;
    margin: 0;
  }
}
</style>
