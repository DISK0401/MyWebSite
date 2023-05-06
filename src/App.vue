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
  right:5%;
  left:5%;
  background-color: blue;
}
main {
  width: 100%;
  margin-top:50px;
  background-color: red;
  /* padding-top: 1.5rem;
  padding-bottom: 0.8rem; */
}
footer {
  position: fixed;
  bottom: 0;
  height: 25px;
  right:5%;
  left:5%;
  background-color: blueviolet;
}
footer #copy {
  text-align: center;
}
</style>
