<template>
  <div class="table">
    合并单元格
  </div>
</template>

<script>
export default {
  name: 'table',
  data () {
    return {
      checkBtn: '上海',
      lab:'上海'
    }
  },
  methods:{
    changeBtn(){
      this.lab = this.checkBtn
    },
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
