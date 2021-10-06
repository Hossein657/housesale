<template>
  <header class="header mb">
    <div class="content">
      <h2>Quality home services,<br> on demand</h2>
      <p class="mb">Experienced, hand-picked Professionals to serve you at your doorstep</p>

      <Searchform/>
    </div>
  </header>

  <div class="container">
    <Cards/>
    <!-- <whyus/> -->

  </div>
</template>

<script>
  import Searchform from '../components/Searchform.vue'
  import Cards from '../components/Cards.vue'
  import Whyus from '../components/Whyus.vue'

export default {
  name: "Home",
  components: {
    Searchform,
    Cards,
    Whyus,
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
    margin-bottom: 20px;
  }

  .content p{
    color: #fff;
    font-size:29px
  }
  .mb{
    margin-bottom: 80px;
  }
</style>
