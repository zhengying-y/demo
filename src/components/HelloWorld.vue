<template>
  <div class="hello">
    <vxe-table
    border
    show-header-overflow
    show-overflow
    highlight-hover-row
    :align="allAlign"
    :data="tableData">
    <vxe-table-column type="seq" title="序号" width="60"></vxe-table-column>
    <vxe-table-column field="name" title="Name"></vxe-table-column>
    <vxe-table-column field="sex" title="Sex"></vxe-table-column>
    <vxe-table-column field="age" title="Age"></vxe-table-column>
    <vxe-table-column field="address" title="Address"></vxe-table-column>
  </vxe-table>
  </div>
</template>


<script>
  
export default {
  name: 'HelloWorld',
  data () {
      return {
        allAlign: null,
        tableData: [
          { id: 10001, name: 'Test1', role: 'Develop', sex: 'Man', age: 28, address: 'vxe-table 从入门到放弃' },
          { id: 10002, name: 'Test2', role: 'Test', sex: 'Women', age: 22, address: 'Guangzhou' },
          { id: 10003, name: 'Test3', role: 'PM', sex: 'Man', age: 32, address: 'Shanghai' },
          { id: 10004, name: 'Test4', role: 'Designer', sex: 'Women ', age: 24, address: 'Shanghai' }
        ]
      }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.hello{
  margin-top: 50px;
  width: 100%;
}
</style>
