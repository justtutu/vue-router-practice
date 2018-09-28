<template>
  <div>

    <el-row>
      <el-col :span="24">
        <el-button type="text">默认按钮</el-button>
        <el-button type="primary">primary button</el-button>
        <el-button type="success">success</el-button>
        <el-button type="danger">danger</el-button>
      </el-col>
      <el-col :span="24">
        <el-button type
                   plain>plain</el-button>
        <el-button type="success"
                   round>round</el-button>
        <el-button type="primary"
                   circle
                   icon="el-icon-edit"></el-button>
      </el-col>
      <el-col :span="24">
        <el-button type="info"
                   disabled="true">disabled</el-button>
        <el-button type="text">text按钮</el-button>
        <el-button-group>
          <el-button type="primary"
                     icon="el-icon-arrow-left">上一页</el-button>
          <el-button type="primary"
                     icon="el-icon-arrow-right">上一页</el-button>
        </el-button-group>
        <el-button type="info"
                   loading="true">loading</el-button>
        <el-button type="danger"
                   @click="doClose">debbuger</el-button>
        <el-button type="primary"
                   @click="doTell">tell</el-button>

      </el-col>
    </el-row>
  </div>

</template>

<script>
export default {
  created () { },
  methods: {
    doClose () {
      let a = 1
      let b = 2
      let c = a + b
      console.log(c);
    },
    doTell () {
      console.log('hehe');
    }
  }
}
</script>

<style>
</style>
