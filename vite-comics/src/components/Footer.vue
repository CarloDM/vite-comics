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
    <div class="container">
      <div class=" sign debug">
        <a class="button debug">SIGN-UP NOW!</a>
      </div>
  
      <div class="follow debug">
        <a href="#">FOLLOW US</a>
        <a href="#"><img src="../assets/vue-dc-comics-1/img/footer-facebook.png" alt=""></a>
        <a href="#"><img src="../assets/vue-dc-comics-1/img/footer-periscope.png" alt=""></a>
        <a href="#"><img src="../assets/vue-dc-comics-1/img/footer-pinterest.png" alt=""></a>
        <a href="#"><img src="../assets/vue-dc-comics-1/img/footer-twitter.png" alt=""></a>
        <a href="#"><img src="../assets/vue-dc-comics-1/img/footer-youtube.png" alt=""></a>
      </div>
    </div>
  </footer>
  
</template>


<style lang="scss" scoped>
@use '../scss/general.scss' as *;

footer{
  width: 100%;
  height: 80px;
}
footer .container{
  @include FlexCenter;
}

.sign{
  @include FlexCenter;
  justify-content: center;
  width: 120px;
  height: 100%;
  .button{
    border: 1px solid rgb(2, 130, 249);
    font-size: 0.8rem;
    // width: 80%;
    // height: 50%;
    padding: 5px 10px;
  }
}

.follow{
  @include FlexCenter;
  justify-content: space-around;
  min-width: 300px;
  height: 100%;

  a{  
    @include FlexCenter;
    margin: 0px 5px;
    color: rgb(2, 130, 249) ;

    img{
      width: 70%;
    }
  }
}

</style>