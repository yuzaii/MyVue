<template>
  <!--组建的结构-->
  <div class="demo">
    <h2>学校名称：{{ schoolname }}</h2>
    <h2>学校地址：{{ schooladr }}</h2>
    <button @click="showname">点我提示学校名</button>
  </div>
</template>

<script>
// 组件交互的相关代码
//创建school组件
export default Vue.extend({
  name: 'School',
  // el: "#app", // 不能写el配置项 vm配置
  data() {
    return {
      schoolname: "北京大学",
      schooladr: "北京"
    }
  },methods: {
    showname(){
      alert(this.schoolname)
    }
  },
})
// export default school
</script>
<style>
/*组件的样式*/
.demo{
  background-color: aquamarine;
}
</style>
