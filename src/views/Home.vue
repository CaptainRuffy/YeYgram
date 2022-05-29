<template>
  <div class="home">
    <!--<img alt="Vue logo" src="../assets/logo.png" /> -->

   
    <card v-for="(post, n) in posts" :key="n" :post="post" />
  </div>
</template>

<script>
// @ is an alias to /src
import card from "@/components/card.vue";
import Vue from "vue";

let posts = [
{
    authorname:"Олег Тинькофф",
    postpictureUrl:"https://i.ytimg.com/vi/U1VwBGCIZao/maxresdefault.jpg",
    authorAvatarUrl:"https://uznayvse.ru/images/content/2021/2/uzn_16123338292.jpg",
    countlikes:193,
    description:"Оформил себе красотульку!",
          },
          {
    authorname:"",
    postpictureUrl:"https://i.ytimg.com/vi/U1VwBGCIZao/maxresdefault.jpg",
    authorAvatarUrl:"https://uznayvse.ru/images/content/2021/2/uzn_16123338292.jpg",
    countlikes:193,
    description:"Оформил себе красотульку!",
          },
          {
    authorname:"Олег Тинькофф",
    postpictureUrl:"https://i.ytimg.com/vi/U1VwBGCIZao/maxresdefault.jpg",
    authorAvatarUrl:"https://uznayvse.ru/images/content/2021/2/uzn_16123338292.jpg",
    countlikes:193,
    description:"Оформил себе красотульку!",
          },
          {
    authorname:"Олег Тинькофф",
    postpictureUrl:"https://i.ytimg.com/vi/U1VwBGCIZao/maxresdefault.jpg",
    authorAvatarUrl:"https://uznayvse.ru/images/content/2021/2/uzn_16123338292.jpg",
    countlikes:193,
    description:"Оформил себе красотульку!",
          },
]

export default Vue.extend({
  name: "Home",
  components: {
    card,
  },

  data() {
    return {posts:posts}
  }
});
</script>
