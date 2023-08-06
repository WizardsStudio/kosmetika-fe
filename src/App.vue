<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
    <nav id="navbar">
      <RouterLink class="nav-item" to="/">o nás</RouterLink>
      <RouterLink class="nav-item" to="/services">služby</RouterLink>
      <RouterLink class="nav-item" to="/">
        <span id="company">kosmetika hanka</span>
      </RouterLink>
      <RouterLink class="nav-item" to="/reservations">rezervace</RouterLink>
      <RouterLink class="nav-item" to="/registration">registrace</RouterLink>
    </nav>
  </header>
  <div id="page-content">
    <RouterView />
  </div>
</template>

<style scoped>
#navbar {
  width: 100%;
  display: flex;
  justify-content: space-around;
}

#page-content {
  margin: 0 9rem;
  margin-top: 3rem;
}
</style>