<template>
  <div id="app">
    <one-header></one-header>
    <one-menu></one-menu>
    <div class="main">
      <router-view></router-view>
    </div>
  </div>
</template>

<script>
  import oneHeader from "./components/header.vue"
  import oneMenu from "./components/menu.vue"
export default {
  name: 'app',
  data:function(){
  	return {show:true}
  },
  components:{
      oneHeader,
      oneMenu
  },
  methods:{
  	toggleMenu:function(){
  		this.show = !show;
  	}
  }
}
</script>
<style>
</style>

