<template>
	<div>
		级别导航
		<el-row>
			<el-col :span="6"></el-col>
		</el-row>
		<el-row>
		<el-col :span="12">
	    <h5>房间列表</h5>
	    <el-menu mode="vertical" default-active="1" class="el-menu-vertical-demo">
	      <el-menu-item-group title="青铜组">
	        <el-menu-item index="1"><i class="el-icon-document"></i>青铜一</el-menu-item>
	        <el-menu-item index="2"><i class="el-icon-document"></i>青铜二</el-menu-item>
	      </el-menu-item-group>
	      <el-menu-item-group title="白银二">
	        <el-menu-item index="3"><i class="el-icon-document"></i>白银一</el-menu-item>
	        <el-menu-item index="4"><i class="el-icon-document"></i>白银二</el-menu-item>
	      </el-menu-item-group>
	    </el-menu>
  		</el-col>
  		<el-row>
			<el-col :span="6"></el-col>
		</el-row>
	</el-row>
	</div>
</template>