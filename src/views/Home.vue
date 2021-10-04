<template>
  <header class="header">
    <div class="content">
      <h2>Quality home services,<br> on demand</h2>
      <p class="mb">Experienced, hand-picked Professionals to serve you at your doorstep</p>

      <Searchform/>
    </div>
  </header>
</template>

<script>
  import Searchform from '../components/Searchform.vue'

export default {
  name: "Home",
  components: {
    Searchform,
  },
};
</script>


<style scoped>

  .header .content {
    position: absolute;
    top: 20%; left: 10%;
  }

  .header{
    height: 90vh;
    background-image: url('../assets/headpic.png');
    background-size: cover;
    position: relative;
    /* z-index: -1; */
  }

  h2{
    color: #fff;
    font-size: 70px;
    font-weight: bold;
  }

  p{
    color: #fff;
    font-size:29px
  }
  .mb{
    margin-bottom: 80px;
  }
</style>
