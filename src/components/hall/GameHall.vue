<template>
<div>
	<el-row style="margin-bottom: 18px">
			<el-col :span='6'>
				<levelnav/>
			</el-col>
			<el-col :span='18'>
				<roomlist/>
			</el-col>
	</el-row>
	
</div>
		
</template>
<script>
import Levelnav from './Levelnav'
import RoomList from './RoomList'
	export default {
  		components:{
  			levelnav:Levelnav,
  			roomlist:RoomList
  		}
	}
</script>