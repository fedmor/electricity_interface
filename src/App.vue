<template>

  <el-container>
    <el-header height="100px" align="center">
      <el-row :gutter="20">
        <el-col :span="6" :offset="1">
          <div class="grid-content " style="font-size: 50px">
            寝室水电查询
          </div>
        </el-col>
      </el-row>

    </el-header>
    <el-main>
      <el-row :gutter="20">
        <el-col :span="10" :offset="1">
          <el-row>
            <div class="grid-content"  style="font-size: 30px">宿舍总有电量</div>
          </el-row>
          <LineChart/>
        </el-col>

        <el-col :span="10" :offset="1">
          <el-row>
          <div class="grid-content "  style="font-size: 30px">宿舍电量查询</div>
          </el-row>
          <SearchTable />

        </el-col>

      </el-row>

    </el-main>
  </el-container>

</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import LineChart from './components/linechart.vue'
import SearchTable from "@/components/SearchTable";

export default {
  name: 'App',
  components: {
    LineChart,
    SearchTable
  },


}
</script>

<style>
/*#app {*/
/*  font-family: Avenir, Helvetica, Arial, sans-serif;*/
/*  -webkit-font-smoothing: antialiased;*/
/*  -moz-osx-font-smoothing: grayscale;*/
/*  text-align: center;*/
/*  color: #2c3e50;*/
/*  margin-top: 60px;*/
/*}*/
.el-header, .el-footer {
  background-color: #ffffff;
  color: #050505;
  text-align: left;
  line-height: 100px;
  border-radius: 2px
}

.el-row {
  margin-bottom: 20px;
}

.el-row:last-child {
  margin-bottom: 0;
}

.el-col {
  border-radius: 4px;
}

.bg-purple-dark {
  background: #99a9bf;
}

.bg-purple {
  background: #d3dce6;
}

.bg-purple-light {
  background: #e5e9f2;
}

.grid-content {
  border-radius: 4px;
  min-height: 36px;
}

.row-bg {
  padding: 10px 0;
  background-color: #f9fafc;
}
</style>
