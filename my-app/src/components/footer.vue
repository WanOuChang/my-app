<template>
<div class="footer">
    <router-link tag="span" to="/home">首页</router-link>
    <router-link tag="span" to="/my">我的</router-link>
</div>
  
</template>

<script>
export default {

}
</script>
<style>

</style>
<style >
.footer{
    width: 100%;
    height: 50px;
    display: flex;
    justify-content: space-around;
    align-items: center;
    border-top:1px solid #ccc;
}
span{
    padding:0 10px;
}
.router-link-active{
    color:red;
}
</style>