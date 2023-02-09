<template>
  <div id="app">
    <Nav></Nav>
    <Banner></Banner>
  </div>
</template>

<script>
import '@/styles/base.css'
import Nav from '@/components/nav/index.vue'
import Banner from '@/components/banner/index.vue'
export default {
  name: 'App',
  components: {
    Nav,
    Banner
  }
}
</script>

<style></style>
