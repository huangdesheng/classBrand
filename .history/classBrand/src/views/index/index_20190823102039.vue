<template>
  <div id="index">
    <header>
      <ul>
        <li>
          <span></span>
          <div>
            <h1>黄村幼儿园</h1>
            <p>地点: 广州黄村</p>
          </div>
        </li>
        <li>
          <div>17:39</div>
          <div>
            <p>星期一</p>
            <p>2019年8月19日</p>
          </div>
          <div>
            <p>30℃</p>
            <p>多云转晴</p>
          </div>
        </li>
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
.img {
  width: 1rem;
  height: 1rem;
  background-size: 100% 100%;
  background-position: center center;
  background-repeat: no-repeat;
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
      width: 97%;
      height: 100%;
      margin: 0 auto;
      display: flex;
      justify-content: space-between;
      align-items: center;
      li {
        .flex;
        &:nth-of-type(1) {
          > span {
            background: url(../../assets/icon/index.png);
            .img;
            margin-right: 0.4rem;
          }
          > div {
            h1 {
              font-size: 0.45rem;
              font-family: Alibaba PuHuiTi;
              font-weight: 500;
              color: rgba(46, 46, 46, 1);
            }
            p {
              font-family: Alibaba PuHuiTi;
              font-weight: 500;
              color: rgba(102, 102, 102, 1);
              font-size: 0.35rem;
              margin-top: 0.2rem;
            }
          }
        }
      }
    }
  }
  section {
    .flex;
    width: 100%;
    margin-top: 1.5%;
    height: 87%;
    aside {
      .bt;
      height: 100%;
      &:nth-of-type(1) {
        width: 40%;
        margin-right: 1.5%;
      }
      &:nth-of-type(2) {
        flex: 1;
      }
    }
  }
}
</style>