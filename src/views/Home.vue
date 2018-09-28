<template>
  <div class="home">
    <el-container>
      <el-aside width="200px">
        <el-menu default-active="2"
                 class="el-menu-vertical-demo"
                 @open="handleOpen"
                 @close="handleClose"
                 background-color="#545c64"
                 text-color="#fff"
                 active-text-color="#ffd04b">
          <el-submenu index="1">
            <template slot="title">
              <i class="el-icon-location"></i>
              <span>Basic</span>
            </template>
            <el-menu-item-group>
              <el-menu-item index="1-1">
                <router-link to="/layout">layout</router-link>
              </el-menu-item>
              <el-menu-item index="1-2">
                <router-link to="/button">button</router-link>
              </el-menu-item>
              <el-menu-item index="1-3">
                <router-link to="/icon">icon</router-link>
              </el-menu-item>
            </el-menu-item-group>
          </el-submenu>
          <el-submenu index="2">
            <template slot="title">
              <i class="el-icon-document"></i>
              <span>form</span>
            </template>
            <el-menu-item index="2-1">
              <router-link to="/form/radio">radio</router-link>
            </el-menu-item>
            <el-menu-item :index="2-2">
              <router-link to="/form/checkbox">checkbox</router-link>
            </el-menu-item>
          </el-submenu>
          <el-menu-item index="3">
            <i class="el-icon-document"></i>
            <span slot="title">导航三</span>
          </el-menu-item>
          <el-menu-item index="4">
            <i class="el-icon-setting"></i>
            <span slot="title">导航四</span>
          </el-menu-item>
        </el-menu>
      </el-aside>
      <el-container>
        <el-header height="">
        </el-header>
        <el-main height="">

          <router-view></router-view>
        </el-main>
      </el-container>
    </el-container>
  </div>
</template>

<script>
export default {
  name: 'home',
  methods: {
    handleOpen: function () {

    },
    handleClose: function () {

    }
  }
}
</script>
<style lang="stylus" scoped>
a
  display block
  color #ffffff
  text-decoration none
</style>