<template>
  <div id="bar">
    <el-menu :default-active="activeIndex" mode="horizontal" active-text-color="#ffd04b">
      <el-menu-item index="1">
        ホーム
      </el-menu-item>
      <el-menu-item index="2">
        なんか
      </el-menu-item>
    </el-menu>
    <div class="title">
      <span>Connet</span>
    </div>
    <div class="line"></div>
  </div>
</template>

<script>
	export default {
		name: "page-header"
	}
</script>

<style scoped>
#bar{
  display: flex;
  width: 100vw;
  background: white;
  border-bottom: #47494e;
  align-items: center;
  justify-content: space-between;
}
  .title{
    color: orange;
    font-weight: bold;
  }
</style>
