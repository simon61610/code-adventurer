<script setup lang="ts">
</script>

<template>
  <header class="header">
    <div class="logo">MyLogo</div>

    <nav class="nav">
      <router-link to="/">首頁</router-link>
      <router-link to="/about">關於</router-link>
    </nav>
  </header>
</template>

<style scoped lang="scss">
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 16px;
  background: #222;
  color: white;
}

.nav {
  display: flex;
  gap: 16px;
}
</style>