<template>
  <div>
    <router-view></router-view>
    <tab-bar>
      <tab-bar-item link='/home' activeColor='deepPink'>
        <template v-slot:item-icon>
          <img src="~assets/img/tabbar/home.svg"  alt="">
        </template>
        <template v-slot:item-icon-active>
          <img src="~assets/img/tabbar/home_active.svg"  alt="">
        </template>
         <template v-slot:item-text>
            首页
        </template>
      </tab-bar-item>

      <tab-bar-item link='/category' activeColor='deepPink'>
         <template v-slot:item-icon>
          <img src="~assets/img/tabbar/category.svg"  alt="">
        </template>
        <template v-slot:item-icon-active>
          <img src="~assets/img/tabbar/category_active.svg"  alt="">
        </template>
         <template v-slot:item-text>
            分类
        </template>
      </tab-bar-item>

      <tab-bar-item link='/shopcart' activeColor='deepPink'>
         <template v-slot:item-icon>
          <img src="~assets/img/tabbar/shopcart.svg"  alt="">
        </template>
        <template v-slot:item-icon-active>
          <img src="~assets/img/tabbar/shopcart_active.svg"  alt="">
        </template>
         <template v-slot:item-text>
            购物车
        </template>
      </tab-bar-item>

      <tab-bar-item link='/profile' activeColor='deepPink'>
         <template v-slot:item-icon>
          <img src="~assets/img/tabbar/profile.svg"  alt="">
        </template>
        <template v-slot:item-icon-active>
          <img src="~assets/img/tabbar/home_active.svg"  alt="">
        </template>
         <template v-slot:item-text>
            我的
        </template>
      </tab-bar-item>
    </tab-bar>
  </div>
</template>

<script>
import TabBar from "components/common/tabbar/TabBar.vue";
import TabBarItem from "components/common/tabbar/TabBarItem.vue";
export default {
  name: "App",
  components: {
    TabBar,
    TabBarItem,
  },
};
</script>

<style>
@import "assets/css/base.css";
</style>
