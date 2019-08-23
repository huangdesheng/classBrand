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
          <div class="time">17:39</div>
          <div class="week">
            <p>星期一</p>
            <p>2019年8月19日</p>
          </div>
          <div class="weather">
            <p>30℃</p>
            <p>多云转晴</p>
          </div>
        </li>
      </ul>
    </header>
    <section>
      <aside>
        <div class="header">
          <p></p>
          <h1>通知公告</h1>
        </div>
        <div class="section">
          <p class="title">人民网评：习近平的回信凝 ...</p>
          <p class="contain">总有一种力量催人奋进，总有一种精神振奋人心。回味习近平总书记给社会各界群众的回信，殷殷嘱托中刻写着伟大精神总有一种力量催人奋进...</p>
          <p class="mainImg" :style="{backgroundImage: 'url(' + img + ')', backgroundSize:'cover'}"></p>
        </div>
        <div class="more">
          查看更多
          <i></i>
        </div>
      </aside>
      <aside>right</aside>
    </section>
  </div>
</template>

<script>
export default {
  data() {
    return {
      img: require("@/assets/pj/repost.png")
    };
  }
};
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
    height: 13%;
    width: 100%;
    > ul {
      list-style: none;
      width: 92%;
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
              font-size: 0.5rem;
              font-family: Alibaba PuHuiTi;
              font-weight: 600;
              color: rgba(46, 46, 46, 1);
            }
            p {
              font-family: Alibaba PuHuiTi;
              font-weight: 500;
              color: #666666;
              font-size: 0.3rem;
              margin-top: 0.15rem;
            }
          }
        }
        &:nth-of-type(2) {
          div {
            font-family: PingFang SC;
            font-weight: 500;
            margin-left: 0.7rem;
            font-weight: 500;
            font-size: 0.4rem;
            p {
              &:nth-of-type(2) {
                margin-top: 0.2rem;
              }
            }
          }
          .time {
            font-size: 1rem;
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
        position: relative;
        .header {
          width: 80%;
          margin: 0 auto;
          display: flex;
          align-items: center;
          height: 14%;
          > p {
            background: url(../../assets/icon/repost.png);
            .img;
            width: 0.8rem;
            height: 0.8rem;
            margin-right: 0.2rem;
          }
          h1 {
            font-size: 0.5rem;
            font-family: Alibaba PuHuiTi;
            font-weight: 600;
            color: rgba(46, 46, 46, 1);
          }
        }
        .section {
          width: 93%;
          margin: 0 auto;
          .title {
            font-family: PingFang SC;
            font-weight: bold;
            color: rgba(46, 46, 46, 1);
            font-size: 0.4rem;
          }
          .contain {
            font-family: PingFang SC;
            font-weight: 500;
            color: #666666;
            font-size: 0.35rem;
            line-height: 0.8rem;
            margin-top: 0.4rem;
            max-height: 3rem;
            display: -webkit-box;
            -webkit-box-orient: vertical;
            -webkit-line-clamp: 4;
            overflow: hidden;
          }
          .mainImg {
            margin-top: 0.4rem;
            .img;
            width: 100%;
            height: 6rem;
          }
        }
        .more {
          position: absolute;
          bottom: 0;
          right: 0;
          width: 3rem;
          height: 0.8rem;
          background: rgba(0, 0, 0, 0.5);
          border-radius: 0.2rem 0 0.2rem 0;
          display: flex;
          justify-content: center;
          color: #fff;
          font-size: 0.3rem;
          align-items: center;
          i {
            background: url(../../assets/icon/index.png);
            .img;
          }
        }
      }
      &:nth-of-type(2) {
        flex: 1;
      }
    }
  }
}
</style>