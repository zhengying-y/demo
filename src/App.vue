<template>
  <div id="app">
    <div class="main">
      <div>表单</div>
      <Element />
    </div>
    <div class="mains">
      <div>表格</div>
      <HelloWorld />
    </div>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Element from './components/Element.vue'
export default {
  name: 'App',
  components: {
    HelloWorld,
    Element
  }
}
</script>

<style>
#app {
  display: flex;
  justify-content: space-around;
  color: #2c3e50;
  margin-top: 60px;
  font-size: 36px;
}
.main{
  width: 40%;
}
.mains{
  width: 50%;
}
.el-textarea .el-textarea__inner{
  resize: none;
} 
</style>
