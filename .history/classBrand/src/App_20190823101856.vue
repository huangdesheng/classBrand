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
@import "./base.less";
.bt {
  width: 100vw;
  height: 100vh;
  background: url(./assets/bg/bg.png);
  background-size: 100% 100%;
  background-repeat: no-repeat;
  background-position: center;
  position: fixed;
  left: 0;
  top: 0;
  display: flex;
  justify-content: center;
  align-items: center;
}
#app {
  .bt;
}
</style>
