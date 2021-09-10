<template>
 <h1>jd shop</h1>
  <input type="text" placeholder="搜索商品" name="shop" v-model="keyWord">
  <button @click="openNewWindow(keyWord)">Some</button>
</template>

<script>
export default {
  name: "JDShop",
  data(){
    return{
      keyWord: ""
    }
  },
  methods:{
    openNewWindow(searchText){
      window.open('https://www.baidu.com/'+searchText)
    }
    }
}

</script>

<style scoped>

</style>