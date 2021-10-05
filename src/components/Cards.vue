<template>
  <div class="container">
      <div class="card" v-for="content in contents" :key="content.id">
          <img :src="content.img" :alt="content.title">
          <p>{{content.title}}</p>
      </div>
  </div>
</template>

<script>
export default {
    name: "Cards",
    data(){
        return {
            contents: [
                {title: "Same great quality. New lower prices.", img: "~/assets/card1.png", id:"1"},
                {title: "Everyday Essentials, High quality affordable ", img: "~/assets/card2.png", id:"2"},
                {title: "Join the makeover journey ", img: "@/assets/card3.png", id:"3"},
            ],
        }
    }

}
</script>

<style>

</style>