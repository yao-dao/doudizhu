<template>
<div class="div1">
  <el-row>
	 <el-col :span="24" style="margin-bottom:100px">欢迎来到斗地主</el-col>
  </el-row>
   <el-row>
      <el-col :span="8">&nbsp;</el-col>

       <el-row>
            <el-col :span="8" style="border:1px solid #99a9bf;padding:21px">
            <el-form ref="form" name='loginForm'>
                <el-form-item style='text-align: center;margin:0px;'>
                    登录
                </el-form-item>
                <el-form-item label="email:">
                  <el-input placeholder="请输入email" name='email'></el-input>
                </el-form-item>
                <el-form-item label="password:">
                  <el-input placeholder="请输入密码" type="password" name='pwd'></el-input>
                </el-form-item>
                <el-form-item>
                  <el-button type="primary" @click="login">登录</el-button>
                  <router-link to="/register">
                  <el-button >注册</el-button>
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
import {login} from '../vuex/actions/UserAction';

	export default {
	  data() {
	    return {
	      
	    }
	  },
	  methods:{
	  	login:function(e){
	  		login(loginForm,this);
	  	}
	  },
	}
</script>

<style type="text/css">
  .div1{
    width:100%;
    height: 96vh;
    background-image:url("../assets/shouye.jpg"); 
    background-size: cover;
  }
</style>
