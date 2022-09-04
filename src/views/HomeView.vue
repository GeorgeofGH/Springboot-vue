<template>
  <div style="padding: 10px">
    <div style="margin: 10px 0">
<!--      功能区-->
      <el-button type="primary">新增</el-button>
      <el-button type="primary">导入</el-button>
      <el-button type="primary">导出</el-button>
    </div>
<!--      搜索区-->
      <div style="margin: 10px 0">
          <el-input v-model="search" placeholder="关键词" style="width: 40%" />
          <el-button type="primary" style="margin: 8px">查询</el-button>
      </div>
<!--      表格-->
    <el-table :data="tableData" border stripe size="10px">

      <el-table-column prop="date" label="日期" ></el-table-column>
      <el-table-column prop="name" label="名字" ></el-table-column>
      <el-table-column prop="address" label="地址" ></el-table-column>

    </el-table>
  </div>

</template>

<script>

export default {
  name: 'HomeView',
  components: {

  },
  data() {
    return {
        search:'',

      tableData: [
        {
          date: '2016-05-03',
          name: 'Tom',
          address: 'No. 189, Grove St, Los Angeles',
        },
        {
          date: '2016-05-02',
          name: 'Tom',
          address: 'No. 189, Grove St, Los Angeles',
        },
        {
          date: '2016-05-04',
          name: 'Tom',
          address: 'No. 189, Grove St, Los Angeles',
        },
        {
          date: '2016-05-01',
          name: 'Tom',
          address: 'No. 189, Grove St, Los Angeles',
        },
      ]
    }
  },
  methods:{
      handleClick(){

      }
  }
}
</script>
