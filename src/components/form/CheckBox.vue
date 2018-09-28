<template>
  <el-row>
    <el-col :span="12">
      <el-checkbox v-model="check"
                   label="1">记住密码</el-checkbox>

    </el-col>
  </el-row>

</template>

<script>
export default {
  data () {
    return {
      check: true
    }
  }
}
</script>

<style>
</style>
