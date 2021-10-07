<template>
  <div class="nav">
    <ul>
      <h1>housesale</h1>
      <li class="logo"><router-link to="/"><img src="../assets/logo.png" alt=""></router-link></li>
      <li><router-link to="/">On sale</router-link></li>
      <li><router-link to="/">For rent</router-link></li>
      <li><router-link to="/About">About us</router-link></li>
      <li><router-link to="/">Property news</router-link></li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "Navbar",
};
</script>

<style scoped>
  h1{
    display:none;
  }
  .nav{
    background-color: rgba(2, 55, 135, 0.8);
    width: 100%;
    position: fixed;
    z-index: 9;
  }
  .nav ul{
    
    list-style: none;
    color: #fff;
    display: flex;
    align-items: center;
    justify-content: flex-end;
    width:90%;
    margin: 0 auto;
  }
  .nav li{
    margin-left: 20px;
  }
  a{
    text-decoration: none;
    color: white;
    padding:5px 10px;
    border-bottom: 1px solid rgba(255, 255, 255, 0);
    
  }
  .logo a{
    border: none !important;
  }
  a:hover{
    border-bottom: 1px solid rgba(255, 255, 255,1);
    transition: all .2s;
  }
  .logo{
    margin-right: 20%;
    margin-right: auto;
  }
  
</style>
