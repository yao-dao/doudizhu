<template>
	<div>
	<el-row>
		<el-col :span="24" style="margin-bottom:100px">欢迎来到斗地主</el-col>
  	</el-row>
	<el-row>
		<el-col :span="6">&nbsp;</el-col>
			<el-col :span="12" style='align-content: center;border:1px solid #99a9bf;padding: 21px;'>
				<el-form ref="form" name='zhuceForm'>
					<el-form-item style='text-align: center;margin:0px;'>
						注册
					</el-form-item>
				  	<el-form-item >
				    <el-input placeholder="请输入email" class='elInputClass' name='email'></el-input>
				    <el-input placeholder="请输入密码" type='password' name='pwd' class='elInputClass'></el-input>
				    <el-input placeholder="请再次输入密码" type='password'  class='elInputClass'></el-input>
				    <el-input placeholder="请输入昵称" name='nicheng' class='elInputClass'></el-input>
				  	</el-form-item>
				  	<el-form-item style='text-align: center'>
				    <el-button type="primary"@click='register'>注册</el-button>
				    <router-link to="/">
				    	<el-button>返回登陆</el-button>
				    </router-link>
				  	</el-form-item>
				</el-form>
			</el-col>
			<el-col :span="6">&nbsp;</el-col>
	</el-row>
		</div>
</template>
<script>
import {zhuce} from '../../vuex/actions/UserAction'
import {getZhuce} from '../../vuex/getters/UserGetter'

export default {
	data(){
		return{
			data:0
		}
	},
	methods:{		//register方法
		register:function(e){
			zhuce(zhuceForm,this);
		}
	},
	computed:{
		data:getZhuce
	}
}
</script>
<style>
	.elInputClass{
		margin-bottom:15px;
	}
</style>
