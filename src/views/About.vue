<template>
	<!-- 页头 -->
	<el-page-header content="关于页面" @back="goBack" />
  <!-- 标签页 -->
  <el-tabs v-model="activeName" class="demo-tabs" @tab-click="handleClick">
    <el-tab-pane label="测试1" name="first">显示信息</el-tab-pane>
    <el-tab-pane label="测试2" name="second">Config</el-tab-pane>
    <el-tab-pane label="测试3" name="third">Role</el-tab-pane>
    <el-tab-pane label="测试4" name="fourth">Task</el-tab-pane>
  </el-tabs>
  
  <div class="about">
   <!-- <el-empty description="数据为空"></el-empty> -->
    <el-carousel trigger="click" height="150px">
         <el-carousel-item v-for="item in 4" :key="item">
           <h3 class="small">{{ item }}</h3>
         </el-carousel-item>
    </el-carousel>
	
	<!-- 步骤条 -->
	<el-steps :active="2" align-center>
    <el-step title="Step 1" description="Some description"></el-step>
    <el-step title="Step 2" description="Some description"></el-step>
    <el-step title="Step 3" description="Some description"></el-step>
    </el-steps>
	</div>
</template>

<script>
export default {
	name: '关于页面',
	data() {
			return {
				title: 'Hello',
				url: "http://0.0.0.0:8089/static/app/#/mainView",
			}
		},
		onLoad() {
			console.log('关于');
		},
		methods: {
	
		}
	}
	
</script>

<style>
.el-carousel__item h3 {
  color: #475669;
  font-size: 14px;
  opacity: 0.75;
  line-height: 150px;
  margin: 0;
  text-align: center;
}

.el-carousel__item:nth-child(2n) {
  background-color: #99a9bf;
}

.el-carousel__item:nth-child(2n + 1) {
  background-color: #d3dce6;
}
.demo-tabs > .el-tabs__content {
  padding: 32px;
  background-color: #f4f5f7;
  color: #6b778c;
  font-size: 32px;
  font-weight: 600;
}

</style>

<!-- 
 六、处置固定资产
 固定资产处置，即固定资产的终止确认，包括固定资产的出售、报废、毁损、对外投资、非货币性资产交换、债务重组等。
 企业在生产经营过程中，可能将不适用或不需要的固定资产对外出售转让，或因磨损、技术进步等原因对固定资产进行报废、
 -->