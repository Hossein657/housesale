<template>
<div class="wrapper">
  <ul>
    <h3 class="h3">Why HOUSESALE Company?</h3>
    <li>
      <div><img src="../assets/whyus/why1.png"></div>
      <div class="content">
        <h4>Transparent pricing</h4>
        <p>See fixed prices before you book. No hidden charges.</p>
      </div>
    </li>
    <li>
      <div><img src="../assets/whyus/why2.png"></div>
      <div class="content">
        <h4>Experts only</h4>
        <p>Our professionals are well trained and have on-job expertise.</p>
      </div>
    </li>
    <li>
      <div><img src="../assets/whyus/why3.png"></div>
      <div class="content">
        <h4>Fully equipped</h4>
        <p>We bring everything needed to get the job done well.</p>
      </div>
    </li>
  </ul>
  
  <div class="images">
    <img class="image" src="../assets/whyus/Rectangle.png" >
    <img class="image" src="../assets/whyus/why4.png" >
  </div>
</div>
</template>

<script>
export default {
    name: "Whyus",

}
</script>

<style scoped>
h3{
  margin-bottom: 50px;
}
li{
  display: flex;
  align-items: center;
  margin-bottom: 50px;
}
li img{
  width:92px;
  height:92px;
  margin-right: 30px;
}
.images{
  display: flex;
  align-items: center;
  justify-content: flex-end;
}
.wrapper{
  display:grid;
  grid-template-columns: repeat(2, 1fr);
}
</style>