<template>
  <Navbar/>
  <router-view />
</template>


<script>
  import Navbar from "./components/Navbar.vue";

export default {
  components:{
    Navbar,
  },
}
</script>

<style>
#app {
  font-family: 'nunito', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  
}

*{
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

ul{
  list-style: none;
}

 h2{
    color: #fff;
    font-size: 70px;
    font-weight: bold;
    margin-bottom: 20px;
  }

  h3{
    font-size: 36px;
  }
  h4{
    font-size: 29px;
    color: #4A4A4A;
  }
  a{
    color: inherit;
    text-decoration: none;
  }
</style>

