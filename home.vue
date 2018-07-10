<template>
    <div>
      <Myheader tst="武汉">
        <img src="../assets/img/home1.png" alt="" slot="left" class="homeImg1">
        <div slot="search" class="home-top">
          <img src="../assets/img/search.png" alt="" class="homeImg2" @click="list()">
          <input type="text" placeholder="李宇春">
        </div>
        <img src="../assets/img/home2.png" alt="" slot="mid" class="homeImg3">
        <img src="../assets/img/home3.png" alt="" slot="right" class="homeImg4">
      </Myheader>
      <Banner></Banner>
      <NavList></NavList>
      <Overseas></Overseas>
      <PlayMusic></PlayMusic>
      <Tabbar></Tabbar>
    </div>
</template>

<script>
  import Myheader from "../components/myheader"
  import Banner from "../components/banner"
  import NavList from "../components/navList"
  import Overseas from "../components/overseas"
  import PlayMusic from "../components/playMusic"
  import Tabbar from "../components/tabbar"
    export default {
        name: "home",
      components:{
          Myheader,
          Banner,
          NavList,Overseas,PlayMusic,Tabbar
      },
      methods:{
          list:function () {
            this.$router.push('/list')
          }
      }

    }
</script>

<style scoped>

</style>
