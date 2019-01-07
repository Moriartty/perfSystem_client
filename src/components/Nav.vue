<template>
  <el-menu :default-active="activeIndex" class="el-menu-demo" mode="horizontal" @select="handleSelect">
    <template v-for="(nav,key) in navList">
      <el-menu-item v-bind:index="key.toString()">{{nav}}</el-menu-item>
    </template>
  </el-menu>
</template>

<script>
    export default {
      name: "Nav",
      data(){
        return {
          navList:['BigData'],
          activeIndex:'0'
        }
      },
      methods:{
        handleSelect:function(e){
          console.log(e);
        }
      }
    }
</script>

<style scoped>

</style>
