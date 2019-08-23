<template>
  <div id="index">
    <header>
      <ul>
        <li>left</li>
        <li>right</li>
      </ul>
    </header>
    <section>
      <aside>left</aside>
      <aside>right</aside>
    </section>
  </div>
</template>

<script>
export default {};
</script>

<style lang="less" scoped>
.bt {
  background: rgba(255, 255, 255, 1);
  box-shadow: 0px 2px 7px 0px rgba(161, 157, 157, 0.23);
  opacity: 0.84;
  border-radius: 10px;
}
.flex {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
#index {
  width: 95%;
  height: 90%;
  header {
    .bt;
    height: 10%;
    width: 100%;
    > ul {
      list-style: none;
      width: 95%;
      height: 100%;
      margin: 0 auto;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
  }
  section {
    .flex;
    width: 100%;
    margin-top: 3%;
    height: 87%;
    aside {
      .bt;
      height: 100%;
      flex: 1;
      &:nth-of-type(1) {
        width: 40%;
      }
    }
  }
}
</style>