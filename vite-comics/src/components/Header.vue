<script>
export default {
  name: 'Header',
  components: {},
  data( ){
    return {
      logoImg : '../assets/vue-dc-comics-1/img/dc-logo.png',
      links : [
        {name: 'characters',    link:'#', active: false},
        {name: 'comics',        link:'#', active: false},
        {name: 'moves',         link:'#', active: false},
        {name: 'tv',            link:'#', active: false},
        {name: 'games',         link:'#', active: false},
        {name: 'collectibles',  link:'#', active: false},
        {name: 'videos',        link:'#', active: false},
        {name: 'fans',          link:'#', active: false},
        {name: 'news',          link:'#', active: false},
        {name: 'shop',          link:'#', active: false},
      ]
      
    }
  }
}
</script>

<template>
  <div class="header debug">
    <div class="logo debug">
      <img src="../assets/vue-dc-comics-1/img/dc-logo.png" alt="">
    </div>

    <div class="options debug">
      <span v-for="(link, index) in links">{{ link.name }}</span>

    </div>

  </div>
  
</template>


<style scoped>
.header{
  display: flex;
  justify-content: space-between;
  width: 100%;
  height: 80px;
}

.logo{

  width: 80px;
  height: 80px;
}

.logo img {
  width: 100%;
}
.options{
  display: flex;
  align-items: center;
}

.options span{
  display: inline-block;
  margin:5px
}
</style>