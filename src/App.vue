<template>
  <div>
    <Navbar :logo="logo_src" :alt="app_name"/>
    <router-view/>
    <Footer/>
  </div>
</template>

<script>
  import Navbar from './components/Navbar';
  import Footer from './components/Footer';

  export default {
    data() {
      return {
        logo_src: "/img/logo.png",
        app_name: "Make Your Buguer"
      }
    },
    components: {
      Navbar,
      Footer
    }
  }
</script>

<style>
  *{
    font-family: Helvetica;
    padding: 0;
    margin: 0;
    box-sizing: border-box;
  }

  .main-container {
    margin: 50px;
    min-height: 250px;
  }

  h1 {
    text-align: center;
    font-size: 42px;
    margin-top: 30px;
    color: #222;
  }
</style>
