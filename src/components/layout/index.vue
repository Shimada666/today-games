<script lang="ts" setup>
import Nav from '@/components/layout/Nav.vue'
</script>

<template>
  <div>
    <Nav />
    <router-view />
    <div class="my-4 text-sm text-center">
      <a href="https://beian.miit.gov.cn/" target="_blank">渝ICP备2020011666号-1</a>
    </div>
  </div>
</template>

<style scoped lang="scss">

</style>
