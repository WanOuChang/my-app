<template>
  <div>
      <div class="banner">
        <div class="swiper-container">
          <div class="swiper-wrapper">
            <div class="swiper-slide">轮播图1</div>
            <div class="swiper-slide">轮播图2</div>
            <div class="swiper-slide">轮播图3</div>
            <div class="swiper-slide">轮播图4</div>
          </div>
        </div>
      </div>
      <div class="main">
        <List v-for="(item,index) in list" :key="index" :item="item"/>
      </div> 
  </div>
</template>

<script>
import List from "../../components/list"
import Swiper from "swiper";
export default {
  created(){
    let mySwiper = new Swiper(
      ".swiper-container",{
        autoplay:true
      }
    );
  },
  components:{
    List,
  },
  data(){
    return{
      list:[
        {
          id:1,
          url:"",
          title:"成单奖励",
        },{
          id:2,
          url:"",
          title:"成单奖励",
        },{
          id:3,
          url:"",
          title:"成单奖励",
        },{
          id:4,
          url:"",
          title:"成单奖励",
        },{
          id:5,
          url:"",
          title:"成单奖励",
        },{
          id:6,
          url:"",
          title:"成单奖励",
        },{
          id:7,
          url:"",
          title:"成单奖励",
        },{
          id:8,
          url:"",
          title:"成单奖励",
        },
      ]
    }
  }
}
</script>

<style lang="scss" scoped>

</style>