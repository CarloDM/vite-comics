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