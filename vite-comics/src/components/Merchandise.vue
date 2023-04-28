<script>
export default {
  name: 'Header',
  components: {},
  data( ){
    return {
      
    }
  }
}
</script>

<template>
  <div class="merch">
    <div v-for="item in 5" :key="item" 
    class="merch_item debug">
      <img src="../assets/vue-dc-comics-1/img/buy-comics-digital-comics.png" alt="">
      <span>DIGITAL COMICS</span>
    </div>

  </div>
</template>


<style scoped>
.merch{
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 100%;
  min-height: 150px;
  background-color: rgb(2, 130, 249);
}
img{
  width: 50px;
}

.merch_item{
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: calc(100% / 5);
}

</style>