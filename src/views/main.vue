<template>
	<!-- 页头 -->
	<el-page-header content="我的" @back="goBack" />
	<div class="about">
		<!-- 头像 -->
	<!-- <el-avatar :size="50" src="https://shadow.elemecdn.com/app/element/hamburger.9cf7b091-55e9-11e9-a976-7f4d0b07eef6.png"></el-avatar> -->
	
	<!-- 卡片 -->
	<el-card class="box-card">
      <div class="card-header">
        <span>头像</span>
		<el-avatar :size="50" src="https://shadow.elemecdn.com/app/element/hamburger.9cf7b091-55e9-11e9-a976-7f4d0b07eef6.png"></el-avatar>
      </div>
    </el-card>

	</div>
</template>

<script>
export default {
  components: {
  }
}
</script>

<style>
.card-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
</style>
