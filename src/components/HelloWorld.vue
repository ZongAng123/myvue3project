<template>
	<!-- 页头 -->
  <el-page-header content="登录页面" @back="goBack" />
  <div class="hello">
	<div class="common-layout">
		<!-- 输入框 -->
	<el-input v-model="input" placeholder="请输入账号" />
	
	<!-- 按钮及 router-link跳转-->
	<router-link to="/about">
		<el-button class="btnsty" type="primary">登录</el-button>
	</router-link>
	</div>
	
	
  </div>

	
</template>

<script>
export default {

  name: 'HelloWorld',
  props: {
    msg: String
  },
  methods:{
     
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.btnsty{ 
/* 登录按钮 */
	background-color: #fd6666;
	top: 40rpx;
}


</style>
