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
  background-size: containb;
  background-repeat: no-repeat;
  background-position: center;
  position: fixed;
  left: 0;
  top: 0;
}
#app {
  .bt;
}
</style>
