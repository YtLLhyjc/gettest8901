<template>
  <div class="listWarp">
    <Myheader txt="取消" class="p2">
      <div slot="search" class="home-top">
        <img src="../assets/img/search.png" alt="" class="homeImg2" @click="list()">
        <input type="text" placeholder="李宇春">
        <img src="../assets/img/list-top.png" alt="" class="listImg">
      </div>
    </Myheader>
    <Stars></Stars>
  </div>
</template>

<script>
  import Myheader from '../components/myheader'
  import Stars from '../components/stars'

    export default {
        name: "list",
      components:{
          Myheader,Stars
      }
    }
</script>

<style scoped>
</style>
