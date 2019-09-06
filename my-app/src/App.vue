<template>
  <div id="app">
    <div class="wrap">
      <router-view/>
    </div>
    
    <Footer/>
  </div>
  
</template>
<script>
import Footer from "./components/footer"
export default {
  components:{
    Footer,
  }
}
</script>

<style lang="scss">
*{
  margin: 0;
  padding: 0;
  list-style: none;
  text-decoration: none;
  box-sizing: border-box;
}
#app, html, body  {
  width: 100%;
  height: 100%;
}
#app{
  display: flex;
  flex-direction: column;
}
.wrap{
  width: 100%;
  flex:1,
}
</style>
