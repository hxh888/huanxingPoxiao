<template>
  <div class="navBar">
    <el-radio-group v-model="checkBtn" @change="changeBtn">
      <el-radio-button v-for="item in data" :key="item.id" :label="item.name">
        <router-link :to="item.path">{{item.name}}</router-link>
      </el-radio-button>
    </el-radio-group>
    <!-- {{checkBtn}}333 -->
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
        checkBtn: '首页',
        data:[
            {path:"/",name:"首页",id:0},
            {path:"/table",name:"合并单元格",id:1}
        ]
    }
  },
  methods:{
    changeBtn(){
        
    },
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
