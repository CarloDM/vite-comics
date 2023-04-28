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
  <footer class="debug">
    <div class="sign debug">
      <div class="botton debug"></div>
    </div>

    <div class="follow debug"></div>
  </footer>
  
</template>


<style scoped>
footer{
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 100%;
  height: 80px;
}
.sign{
  width: 120px;
  height: 100%;
}
.follow{
  min-width: 300px;
  height: 100%;
}

</style>