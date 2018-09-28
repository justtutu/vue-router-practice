<template>
  <div>
    <h4>radio</h4>
    <el-radio v-model="sex"
              label="1">男</el-radio>
    <el-radio v-model="sex"
              label="2">女</el-radio>
    <el-radio v-model="sex"
              label="3"
              :disabled="true"></el-radio>
    <h4>radio按钮组</h4>
    <el-radio-group v-model="radio2">
      <el-radio v-for="item in radios"
                :key="item.key"
                :label="item.label">
        {{item.title}}
        
      </el-radio>
    </el-radio-group>
  </div>

</template>





<script>
export default {
  data () {
    return {
      sex: 1,
      radio2: '2',
      radios: [
        {
          key: '1',
          label: '1',
          title: '北京'
        },
        {
          key: '2',
          label: '2',
          title: '上海'
        }
      ]
    }
  }
}
</script>

<style>
</style>
