<template>
  <div id="app">
    <Header/>
    <Main/>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'


export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer
  }
}
</script>

<style lang="scss">
@import 'src/assets/style.scss';

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  color: $my-color-edward;
  section{
    padding: 150px 0;
  }
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
  input,textarea,select{
    border: none;
    color: rgb(105, 104, 104);
    padding: 0.8rem 0.8rem;
    border-radius: 0.2rem;
  }
  button{
    padding: 10px 25px;
    border:  $my-color-blue-lagoon solid 2px;
    border-radius: 0.25rem;
  }
  button:hover{
      transition: background-color, border;
      transition-duration: 0.5s;
      border:  $my-color-green-hover solid 2px;
      border-radius: 0.25rem;
      background-color:$my-color-green-hover;
  }
  ul{
    list-style: none;
    margin: 0;
    padding: 0;
  }
  .my-card{
    padding: 30px;
    border-radius: 0.5rem;
    i{
      margin-bottom: 1rem;
      font-size: 1.5rem;
    }
  }
}
</style>
