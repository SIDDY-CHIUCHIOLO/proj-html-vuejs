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
  color: $my-color-edward;
  p{
    margin: 0;
  }
  h1, h2, h3, h4, h5{
    font-weight: bold;
  }
  a{
    text-decoration: none;
    color: $my-color-edward;
  }
  ul{
    list-style: none;
    margin: 0;
  }
  button{
    color: white;
    padding: 10px 25px;
    border:  $my-color-blue-lagoon solid 2px;
    border-radius: 0.25rem;
  }
  .my-card{
    padding: 30px;
    border-radius: 0.5rem;
  }
}
</style>
