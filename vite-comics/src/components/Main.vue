<script>
import cardsSpec from '../data/dc-comics.json';
import Card from "../components/card.vue";
export default {
  name: 'Header',
  components: {Card},
  data( ){
    return {
      cardsSpec,
    }
  }
}
</script>

<template>
  <div class="main">
    <div class="container">
      <Card class="card" 
      v-for="(card, index) in cardsSpec" :key="index"
      :thumb="card.thumb"
      :title="card.series"
      />
    </div>
  </div>
</template>


<style lang="scss" scoped>
@use '../scss/general.scss' as *;

.main{
  width: 100%;

}

.main .container {
  display: flex;
  flex-wrap: wrap;
}

</style>