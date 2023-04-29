<script>
import cards from '../data/dc-comics.json'
export default {
  name:'card',
  data(){
    return{
      cards,
    }
  },
  methods:{
    getImage(img){
      return new URL(`../assets/${img}`, import.meta.url).href
    }
  }
}
</script>

<template>
  <div id="card" class="debug" v-for="(card,index) in cards" :key="index">
    <img :src= card.thumb alt="" class="debug">
    <h4>{{ card.series }}</h4>
  </div>
</template>

<style lang="scss" scoped>
@use '../scss/general.scss' as *;

#card {
  width: calc(100% / 6);
  height: calc (50% / 2);
  padding: 5px;


  img{
    width: 100%;
    aspect-ratio: 1/1;
  }
  h4 {
    font-size: 0.7rem;
    font-weight: 400;
    line-height: 100%;
  }
}

</style>