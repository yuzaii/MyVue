<template>
<div>
  <school></school>
  <student> </student>
</div>
</template>

<script>
// 引入组件
import School from "./School";
import Student from "./Student";
export default {
  name: "App",
  components:{
  School,Student
  }
}
</script>

<style scoped>

</style>
