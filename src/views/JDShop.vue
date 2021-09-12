<template>
  <div class="d-flex align-items-center justify-content-center" style="height:70vh;">
    <div class="card" style="width:15rem;height:20rem;">
      <div class="card-header text-center">JDShop</div>
      <div class="card-body justify-content-center align-items-center">
        <form class="text-center" >
          <textarea class="form-control text-center"  type="text" placeholder="搜索商品" name="shop" v-model="keyWord" style="height:5rem;"></textarea>
          <br />
          <button class="btn btn-primary" type="submit" @click="openNewWindow()">开始</button>
          <hr />
          <button @click="openEncode()" class="btn btn-primary">GBK</button>
        </form>
      </div>
    </div>
  </div>
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
    openNewWindow: function(){
      window.open(`https://www.gwdang.com/search?keyword=${this.keyWord}&paara_get=&pg=&sort=0&class_keyword=&pub=1&site_id=3&quan=&tag_id=4&ingredient=&ingList=`)
    },
    openEncode: function(){
      window.open('https://tool.chinaz.com/tools/urlencode.aspx')
    }
    }
}

</script>

<style scoped>

</style>