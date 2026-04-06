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
