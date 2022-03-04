<script lang="ts" setup>
import Logo from '@/components/Logo.vue'
</script>

<template>
  <div class="nav">
    <div class="nav-inner response-wrap">
      <span class="text-xl font-extrabold pt-1">摸鱼 - 今天玩什么</span>
      <Logo :width="24" />
    </div>
  </div>
</template>

<style scoped lang="scss">
.nav {
  border-bottom: 1px solid #f0f0f0;
  .nav-inner {
    display: flex;
    align-items: center;
    justify-content: space-between;

    height: 48px;
  }
}
</style>
