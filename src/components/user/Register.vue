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
                		注册
            </el-form-item>
                <el-input placeholder="请输入email" style="margin-bottom: 					6px;"></el-input>
              </el-form-item>
                <el-input placeholder="请输入密码" style="margin-bottom: 					6px;"></el-input>
              </el-form-item>
                <el-input placeholder="请再次密码" style="margin-bottom: 					6px;"></el-input>
              </el-form-item>
                <el-input placeholder="请输入昵称" style="margin-bottom: 					6px;"></el-input>
              </el-form-item>
              <el-form-item>
                <el-button type="primary" @click="onSubmit">注册</el-button>
                <router-link to="/">
                <el-button>返回登录</el-button>
                </router-link>
              </el-form-item>
            </el-form>
            </el-col>
        </el-row>
      </el-col>
    </el-row>
      <el-row>
      <el-col :span="8">&nbsp;</el-col>
      </el-row>
      </el-row>
	 </el-row>
	</div>
</template>