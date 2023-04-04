<template>
  <div class="web-ssh-div">
    <el-form ref="form" :inline="true" :model="form" label-width="80px">
      <el-form-item label="地址">
        <el-input v-model="form.address"></el-input>
      </el-form-item>
       <el-form-item label="端口">
        <el-input v-model="form.port"></el-input>
      </el-form-item>
       <el-form-item label="用户">
        <el-input v-model="form.user"></el-input>
      </el-form-item>
       <el-form-item label="密码">
        <el-input type="password" v-model="form.psd"></el-input>
      </el-form-item>

    </el-form>
    <p style="text-align:right;">
         <el-button type="primary">连接</el-button>
         <el-button type="primary">关闭连接</el-button>
         <el-button type="primary">清理终端</el-button>
      </p>
  </div>
</template>
<script>
export default {
    data() {
      return {
        form: {
          address: '',
          port: '',
          user: '',
          psd: '',
        }
      }
    },
}
</script>
<style scoped>
.web-ssh-div{
    background:#000;
    height: 764px;
    padding:10px;
}
</style>
