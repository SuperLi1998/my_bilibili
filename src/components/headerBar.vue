<template>
  <div class="header_bar">
    <ul class="bar_left">
      <li>
        <a href="http://www.bilibili.com" class="default">
          <span class="logo"><img src="../assets/bilibili.png" alt="" /></span>
          <span>首页</span>
        </a>
      </li>
      <li>
        <a href="http://www.bilibili.com" class="default">
          <span>番剧</span>
        </a>
      </li>
      <li>
        <a href="http://www.bilibili.com" class="default">
          <span>直播</span>
        </a>
      </li>
      <li>
        <a href="http://www.bilibili.com" class="default">
          <span>游戏中心</span>
        </a>
      </li>
      <li>
        <a href="http://www.bilibili.com" class="default">
          <span>会员购</span>
        </a>
      </li>
      <li>
        <a href="http://www.bilibili.com" class="default">
          <span>漫画</span>
        </a>
      </li>
      <li>
        <a href="http://www.bilibili.com" class="default">
          <span>赛事</span>
        </a>
      </li>
      <li>
        <a href="http://www.bilibili.com" class="default">
          <span>放放假</span>
        </a>
      </li>
      <li>
        <a href="http://www.bilibili.com" class="default">
          <span>记录</span>
        </a>
      </li>
      <li>
        <a href="http://www.bilibili.com" class="default">
          <div class="wrap">
            <span class="logo"
              ><img src="../assets/download-white.png" alt=""
            /></span>
            <span>下载客户端</span>
          </div>
        </a>
      </li>
    </ul>
    <div class="bar_center">
      <div class="search">
        <div class="search-form">
          <div class="content">
            <input type="text" value="柯南" maxlength="100" />
            <div class="clean">
              <img src="../assets/clean.png" alt="" />
            </div>
          </div>

          <div class="search-btn">
            <img src="../assets/search.png" alt="" />
          </div>
        </div>

        <div class="search-panel"></div>
      </div>
    </div>
    <ul class="bar_right">
      <li class="avatarWrap">
        <div class="avatar">
          <img src="../assets/avatar.jpeg" alt="" />
        </div>
      </li>
      <li>
        <a href="#">
          <span class="icon"><img src="../assets/da-white.png" alt="" /></span>
          <span class="text">大会员</span>
        </a>
      </li>
      <li>
        <a href="#">
          <span class="icon"
            ><img src="../assets/xiaoxi-white.png" alt=""
          /></span>
          <span class="text">消息</span>
        </a>
      </li>
      <li>
        <a href="#">
          <span class="icon"
            ><img src="../assets/dongtai-white.png" alt=""
          /></span>
          <span class="text">动态</span>
        </a>
      </li>
      <li>
        <a href="#">
          <span class="icon"
            ><img src="../assets/star-white.png" alt=""
          /></span>
          <span class="text">收藏</span>
        </a>
      </li>
      <li>
        <a href="#">
          <span class="icon"
            ><img src="../assets/history-white.png" alt=""
          /></span>
          <span class="text">历史</span>
        </a>
      </li>
      <li>
        <a href="#">
          <span class="icon"
            ><img src="../assets/chuangzuo-white.png" alt=""
          /></span>
          <span class="text">创作中心</span>
        </a>
      </li>
      <li class="sendWrap">
        <a href="#" class="btn">
          <div class="wrap">
            <span class="send-icon">
              <img src="../assets/send-white.png" alt="" />
            </span>
            <span>投稿</span>
          </div>
        </a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {};
</script>

<style lang="less">
.header_bar {
  box-sizing: border-box;
  display: flex;
  align-items: center;
  justify-content: space-between;
  height: 64px;
  padding: 0 24px;
  background: #000;
  max-width: 2560px;
  width: 100%;
  .bar_left {
    display: flex;
    align-items: center;
    font-size: 14px;
    li {
      display: list-item;
      a {
        display: inline-block;
        margin-right: 15px;
        img {
          margin-right: 6px;
          width: 18px;
          height: 18px;
        }
      }
    }
  }

  .bar_center {
    flex: 1;
    height: 38px;

    .search-form {
      box-sizing: border-box;
      position: relative;
      display: flex;
      align-items: center;
      padding: 0 48px 0 4px;
      border-radius: 8px;
      z-index: 1;
      overflow: hidden;
      line-height: 38px;
      height: 40px;
      border: 1px solid #e3e5e7;
      background-color: #f1f2f3;
      opacity: 0.9;
      transition: background-color 0.3s;
      .content {
        display: flex;
        align-items: center;
        justify-content: space-between;
        position: relative;
        padding: 0 8px;
        width: 100%;
        height: 32px;
        border: 2px solid transparent;
        border-radius: 6px;
        input {
          flex: 1;
          overflow: hidden;
          padding-right: 8px;
          border: none;
          background-color: transparent;
          box-shadow: none;
          color: #61666d;
          font-size: 14px;
          line-height: 20px;
          outline: none;
        }
        .clean {
          visibility: inherit;
          cursor: pointer;
        }
      }

      .search-btn {
        position: absolute;
        top: 3px;
        right: 7px;
        display: flex;
        align-items: center;
        justify-content: center;
        margin: 0;
        padding: 0;
        width: 32px;
        height: 32px;
        border: none;
        border-radius: 6px;
        color: #18191c;
        line-height: 32px;
        cursor: pointer;
        transition: background-color 0.3s;
      }

      .search-btn:hover {
        background-color: #e3e5e7;
      }
    }

    .search-form:hover {
      opacity: 1;
    }
  }

  .bar_right {
    margin-left: 10px;
    display: flex;

    li {
      display: list-item;
      a {
        color: #fff;
        display: flex;
        align-items: center;
        flex-direction: column;
        flex-shrink: 0;
        margin-right: 0;
        min-width: 50px;
        text-align: center;
        font-size: 13px;
        .icon {
          margin-bottom: 2px;
        }
      }
    }

    .avatarWrap {
      padding-right: 10px;
      .avatar {
        width: 38px;
        height: 38px;
        border-radius: 50%;
        overflow: hidden;
        border: 2px solid #fff;
        img {
          width: 100%;
          height: 100%;
        }
      }
    }

    .sendWrap {
      display: flex;
      align-items: center;
      justify-content: center;
      .btn {
        display: inline-block;
        .wrap {
          width: 90px;
          height: 34px;
          background: #fb7299;
          margin-left: 10px;
          color: #fff;
          border-radius: 8px;
          display: flex;
          align-items: center;
          justify-content: center;
          font-weight: 400;
          font-size: 14px;
          vertical-align: bottom;
          .send-icon {
            width: 18px;
            height: 18px;
            margin-right: 4px;

            img {
              width: 100%;
              height: 100%;
            }
          }
        }
      }
    }
  }
}

.default {
  height: 64px;
  line-height: 64px;
  color: #fff;
  font-size: 14px;
  cursor: pointer;
}
</style>
