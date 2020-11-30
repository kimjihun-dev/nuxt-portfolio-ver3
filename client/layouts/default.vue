<template>
  <div id="wrap">
    <AppHeader />
    <Nuxt />
  </div>
</template>

<script>
import AppHeader from '@/components/AppHeader.vue'
export default {
    components: { AppHeader }
}
</script>

<style>
html {
  font-size: 14px;
  font-family: 'Noto Sans KR', sans-serif;
  box-sizing: border-box;
}
*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

#wrap { width: 100%; display: flex; }
@media all and (max-width: 1024px) {
    #wrap { display: flex; flex-flow: column wrap; }
}
</style>
