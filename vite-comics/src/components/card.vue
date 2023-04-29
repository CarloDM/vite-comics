<script>
export default {

}
</script>

<template>
  <div id="card" class="debug">
    <img src="" alt="" class="debug">
    <h4>title</h4>
  </div>
</template>

<style lang="scss" scoped>
@use '../scss/general.scss' as *;

#card {
  width: calc(100% / 6);
  padding: 5px;
  

  img{
    width: 100%;
    aspect-ratio: 1/1;
  }
}

</style>