<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
    <div>ヘッダーです</div>
    <RouterLink :to="{ name: 'home' }">Home</RouterLink>
  </header>
    <main>
      <RouterView />
    </main>
  <footer>
    <div id="copy">&copy; Daisuke Tomioka</div>
  </footer>
</template>

<style scoped>
header {
  position: fixed;
  top: 0;
  height: 50px;
  width: 100%;
}
main {
  width: 100%;
  margin-top:50px;
  /* padding-top: 1.5rem;
  padding-bottom: 0.8rem; */
}
footer {
  position: fixed;
  bottom: 0;
  height: 25px;
  width:100%;
}
footer #copy {
  text-align: center;
}
</style>
