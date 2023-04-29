<script>
export default {
  name:'card',
  props:{
    thumb: String,
    title : String
  },
  data(){
    return{
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
  <div id="card" class="debug">
    <img :src='thumb' alt="" class="debug">
    <h4>{{ title }}</h4>
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