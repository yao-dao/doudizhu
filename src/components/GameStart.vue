<template>
<div>
  <el-row>
	 <el-col :span="24" style="margin-bottom:100px">欢迎来到斗地主</el-col>
  </el-row>
   <el-row>
      <el-col :span="8">&nbsp;</el-col>

       <el-row>
            <el-col :span="8" style="border:1px solid #99a9bf;padding:21px">
            <el-form ref="form">
                <el-form-item style='text-align: center;margin:0px;'>
                    登录
                </el-form-item>
                <el-form-item label="email:">
                  <el-input placeholder="请输入email"></el-input>
                </el-form-item>
                <el-form-item label="password:">
                  <el-input placeholder="请输入密码"></el-input>
                </el-form-item>
                <el-form-item>
                  <el-button type="primary" @click="onSubmit">登录</el-button>
                  <router-link to="/register">
                  <el-button @click="onRegist">注册</el-button>
                  </router-link>
                </el-form-item>
            </el-form>
            </el-col>
       </el-row>

      <el-row>
        <el-col :span="8">&nbsp;</el-col>
      </el-row>
   </el-row>
</div>
</template>
<script>

	export default {
	  data() {
	    return {
	      
	    }
	  }
	}
</script>

