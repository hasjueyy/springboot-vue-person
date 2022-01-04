<template>
  <el-main style="padding: 10px">
    <div style="margin: 10px">
      <el-button type="primary">新增</el-button>
      <el-button type="primary">导入</el-button>
      <el-button type="primary">导出</el-button>
      <el-button type="primary" style="float: right">查找</el-button>
      <el-input v-model='search' placeholder="请输入待搜索的内容" style="width:200px; float:right"></el-input>


    </div>
    <div style="padding: 10px">

    </div>

    <el-table :data="tableData" stripe style="width: 100%" border>
      <el-table-column prop="date" label="Date" sortable/>
      <el-table-column prop="name" label="Name" sortable/>
      <el-table-column prop="address" label="Address" sortable/>
      <el-table-column fixed="right" label="Operations" width="200">
        <template #default>
          <el-button type="text" size="small" @click="handledelete"
          >删除
          </el-button
          >
          <el-button type="text" size="small" @click="handleupdate">修改</el-button>
        </template>
      </el-table-column>
    </el-table>
    <div>
      <div class="demo-pagination-block" style="padding: 10px;float: right">
        <el-pagination
            v-model:currentPage="currentPage4"
            :page-sizes="[5, 10, 20]"
            :page-size="10"
            layout="total, sizes, prev, pager, next, jumper"
            :total="100"
            @size-change="handleSizeChange"
            @current-change="handleCurrentChange"
        >
        </el-pagination>
      </div>
    </div>
  </el-main>
</template>

<script>
export default {
  name: 'Main',
  component: {},
  data() {
    return {
      search: '',
      currentPage4:1,
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
      ],
    }
  },
  methods:{
    handledelete(){

    },
    handleupdate(){

    },
    handleSizeChange(){

    },
    handleCurrentChange(){

    },

  }


}

</script>

<style scoped>

</style>