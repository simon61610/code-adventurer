<script setup lang="ts">
import logo from '@/assets/images/logo.png'
</script>

<template>
  <header class="header">
    <!-- 左邊 -->
    <nav class="nav nav-left">
      <router-link to="/">關於</router-link>
      <router-link to="/portfolio">任務</router-link>
    </nav>

    <!-- 中間 Logo -->
    <router-link to="/" class="logo">
      <img :src="logo" alt="logo" />
    </router-link>

    <!-- 右邊 -->
    <nav class="nav nav-right">
      <router-link to="/blog">魔王</router-link>
      <router-link to="/contact">地圖</router-link>
    </nav>
  </header>
</template>

<style scoped lang="scss">
.header {
  // outline: 1px solid red; // TODO 開發用

  max-width: 1200px;
  margin: 0 auto;
  padding: 0 $spacing-lg;

  // 三欄版型：左 / 中 / 右 -> 1fr = 平分剩餘空間 | auto = 依內容寬度
  display: grid;
  grid-template-columns: 1fr auto 1fr;
  align-items: center;
  gap: $spacing-lg;

  background: $color-bg;
  color: $color-text;

  // nav
  .nav {
    display: flex;
    gap: $spacing-xl;
    font-size: $font-size-lg;
  }

  .nav-left {
    justify-self: end;
  }

  .nav-right {
    justify-self: start;
  }

  // logo
  .logo {
    justify-self: center;

    img {
      max-height: 200px;
      display: block;
    }
  }
}
</style>
