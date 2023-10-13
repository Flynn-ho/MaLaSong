<template>
  <div>
    <div>
      <el-row class="tac">
        <el-col :span="12">
          <h5>马拉松</h5>
          <el-menu default-active="2" class="el-menu-vertical-demo" @open="handleOpen" @close="handleClose">
            <el-submenu index="1">
              <template slot="title">
                <i class="el-icon-location"></i>
                <span>马拉松签到签退</span>
              </template>
              <el-menu-item-group>
                <template slot="title">签到</template>
                <el-menu-item index="1-2">签到
                  <div style="margin-left:50%; margin-top:50%">
                    <el-button type="primary" icon="el-icon-delete-location">签到</el-button>
                  </div>
                </el-menu-item>
                <el-menu-item index="1-1">签退
                  <div style="margin-left:50%;margin-top:50%">
                    <el-button type="warning" icon="el-icon-delete-location">签退</el-button>
                  </div>
                </el-menu-item>
              </el-menu-item-group>
            </el-submenu>
          </el-menu>
        </el-col>
      </el-row>
    </div>
    <div>

    </div>

  </div>
</template>

<script>
export default {
  methods: {
    handleOpen(key, keyPath) {
      console.log(key, keyPath)
    },
    handleClose(key, keyPath) {
      console.log(key, keyPath)
    }
  }
}
</script>

<style>
</style>