<template>
      <tab-bar>
   <tar-bar-item path="/home">
      <img slot="tabBarImg" src="~assets/img/home.png">
     <img slot="tabBarImgActive" src="~assets/img/home-active.png">
       <div slot="tarBarContent">首页</div>
   </tar-bar-item>
    <tar-bar-item path="/category">
      <img slot="tabBarImg" src="~assets/img/category.png">
      <img slot="tabBarImgActive" src="~assets/img/category-active.png">
       <div slot="tarBarContent">分类</div>
   </tar-bar-item>
     <tar-bar-item path="/cart">
      <img slot="tabBarImg" src="~assets/img/cart.png">
     <img slot="tabBarImgActive" src="~assets/img/cart-active.png">
       <div slot="tarBarContent">购物车</div>
   </tar-bar-item>
     <tar-bar-item path="profile">
     <img slot="tabBarImg" src="~assets/img/profile.png">
      <img slot="tabBarImgActive" src="~assets/img/profile-active.png">
       <div slot="tarBarContent">我的</div>
   </tar-bar-item>
  </tab-bar>

</template>

<script>
import TabBar from 'components/common/tarbar/TabBar'
import TarBarItem from "components/common/tarbar/TarBarItem"

export default {
  name: 'mainTarBar',
  components: {
    TabBar,
    TarBarItem
  }
}
</script>
<style>
</style>
