<template>
  <div class="banner w">
    <div class="sidebar"></div>
    <div class="ration">
      <el-carousel trigger="click" height="150px">
        <el-carousel-item v-for="item in 4" :key="item">
          <h3 class="small">{{ item }}</h3>
        </el-carousel-item>
      </el-carousel>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style></style>
