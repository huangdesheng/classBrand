<template>
  <div id="app">
    <router-view />
  </div>
</template>

<script>
export default {
  name: "App"
};
</script>

<style lang="less">
.bt {
  width: 100vw;
  height: 100vh;
  background: url(./assets/bg/bg.png);
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
}
</style>
