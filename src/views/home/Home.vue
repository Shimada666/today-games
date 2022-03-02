<script lang="ts" setup>
import data from '@/views/home/data.json'
</script>

<template>
  <div class="main response-wrap">
    <div class="game-list">
      <div
        v-for="(item, index) in data.gameList"
        :key="index"
        class="game-list-item">
        <div class="item-image">
          <img :src="item.imgUrl" alt="image error">
        </div>
        <div class="item-content">
          <a
            :href="item.gameUrl"
            target="_blank"
            class="item-title">{{ item.title }}</a>
          <div class="item-description">{{ item.description }}</div>
          <!--<div class="item-tags">合成，西瓜</div>-->
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
.main {
  .game-list {
    .game-list-item {
      padding: 24px 0;
      display: flex;
      border-bottom: 1px solid #f0f0f0;
      .item-image {
        width: 90px;
        img {
          width: 100%;
          border-radius: 9999999px;
        }
      }
      .item-content {
        padding-left: 24px;
        .item-title {
          font-weight: 700;
          font-size: 18px;
          color: #404040;
        }
        .item-description {
          font-size: 14px;
          color: #404040;
          margin: 8px 0 12px;
        }
      }
    }
  }
}
</style>
