<script>
import Card from "../components/card.vue";
export default {
  name: 'Header',
  components: {Card},
  data( ){
    return {
      
    }
  }
}
</script>

<template>
  <div class="main">
    <div class="container">
      <Card class="card" 
      v-for="card in 12"/>
    </div>
  </div>
</template>


<style lang="scss" scoped>
@use '../scss/general.scss' as *;

.main{
  width: 100%;
  min-height: 120px;
}

.main .container {
  @include FlexCenter;
  flex-wrap: wrap;
}

.card{

}

</style>