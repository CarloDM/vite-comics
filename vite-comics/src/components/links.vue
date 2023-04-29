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
  <div class="links debug">
    <div class="container">
      
      <section class="debug">
        <div class="col debug">
          <h3>titolo</h3>
          <ul>
            <li v-for="(itemList,index) in 8">list item</li>
          </ul>
        </div>
        <div class="col debug">
          <h3>titolo</h3>
          <ul>
            <li v-for="(itemList,index) in 4">list item</li>
          </ul>
          <h3>titolo</h3>
          <ul>
            <li v-for="(itemList,index) in 4">list item</li>
          </ul>
        </div>
        <div class="col debug">
          <h3>titolo</h3>
          <ul>
            <li v-for="(itemList,index) in 11">list item</li>
          </ul>
        </div>
      </section>
      <div class="logo_bg debug"></div>

    </div>
  </div>
</template>


<style lang="scss" scoped>
@use '../scss/general.scss' as *;

.links{
  display: flex;
  width: 100%;
  height: 250px;
  background-image: url(../assets/vue-dc-comics-1/img/footer-bg.jpg);
  background-size: contain;
}
.links .container {
  @include FlexCenter;
  height: 100%;
}
section{
  display: flex;
  height: 100%;
}
section, .logo_bg {
  width: 50%;
  height: 100%;
}

.col{
  width: calc(100% /4);
  height: 100%;

  h3{
    margin-bottom: 5px;
    color: white;
  }

  ul {
    list-style: none;
    li {
      color: rgb(180, 180, 180);
      font-size: 0.7rem;
      margin-bottom: 3px;
    }
  }
}

.logo_bg {
  background-image: url(../assets/vue-dc-comics-1/img/dc-logo-bg.png);
  background-size: cover;

  background-repeat: no-repeat;
  background-position-y: center;
}



</style>