<template>
  <div id="app">
    <Header/>
    <Main/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'


export default {
  name: 'App',
  components: {
    Header,
    Main,
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
    color: $my-color-grey;
  }
  ul{
    list-style: none;
    margin: 0;
  }
  button{
    color: white;
    padding: 10px 25px;
    border:  #058283 solid 2px;
    border-radius: 3px;
  }
  .my-card{
    padding: 30px;
    border-radius: 0.5rem;
  }
}
</style>
