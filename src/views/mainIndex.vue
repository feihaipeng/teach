<template>
  <div class="mainIndex">
    <el-container  class="containerBox">
      <el-header><headerIndex :name='name' /></el-header>
      <el-container>
        <el-aside width="200px"><asideIndex /></el-aside>
        <el-main><blackBoard /></el-main>
      </el-container>
    </el-container>
    <!-- <message /> -->
  </div>
</template>

<script>
import headerIndex from './../components/header/index'
import asideIndex from './../components/aside/index'
import message from './../components/messageList/index'
import blackBoard from './blackBoard/index'

export default {
  data () {
    return {
      name: '教学系统'
    }
  },
  components: {
    headerIndex,
    asideIndex,
    message,
    blackBoard
  }
}
</script>
<style>
  .mainIndex {
    overflow-x: hidden;
    overflow-y: hidden;
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
  }
  .containerBox {
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
    background: #B3C0D1;
  }
  .el-header, .el-footer {
    padding: 0px !important;
    background-color: #B3C0D1;
    color: #333;
    text-align: center;
    line-height: 60px;
  }

  .el-aside {
    background-color: #D3DCE6;
    color: #333;
    /* text-align: center;
    line-height: 200px; */
  }

  .el-main {
    background-color: #E9EEF3;
    color: #333;
    text-align: center;
    line-height: 160px;
  }
</style>
