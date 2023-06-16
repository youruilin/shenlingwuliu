<!-- 排班设置页 -->
<template>
  <div class="dashboard-container waybill-list customer-list-box">

  </div>
</template>

<script>
export default {

}
</script>

<style rel="stylesheet/scss" lang="scss" scoped>
::v-deep .table-card-box {
  .el-card__body {
    padding-bottom: 0px;
  }
}
::v-deep .pagination{
  padding-bottom: 30px;
}
.tab-box {
  color: #20232a;
  ::v-deep .el-tabs__item.is-active {
    color: #20232a;
    font-size: 16px;
    font-weight: bold;
  }
  ::v-deep .el-form-item__content {
    height: 40px;
  }
  ::v-deep .el-tabs__item {
    font-size: 14px;
  }
  ::v-deep .el-tabs__item:hover {
    color: #20232a;
    font-size: 16px;
    font-weight: bold;
    cursor: pointer;
  }
  ::v-deep .el-tabs__active-bar {
    background-color: #e15536;
  }
  ::v-deep .tips {
    margin-left: 130px;
    margin-bottom: 14px;
    color: #bac0cd;
  }
  .el-checkbox {
    margin-right: 12px;
  }
  ::v-deep .workDay {
    .el-form-item__error {
      position: relative;
    }
  }
}
::v-deep .el-dialog__body {
  padding-top: 30px !important;
  .el-tabs__header {
    padding-bottom: 25px;
  }
}
::v-deep .el-tabs__nav,
.is-top {
  transform: translateX(30px) !important;
}
</style>
