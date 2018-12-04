<template>
  <div class="contain">
    <!--头部-->
    <div class="top">
      <ul>
        <li>
          <a href="#" class="person"></a>
        </li>
        <li>
          <a href="#">qq音乐</a>
        </li>
        <li>
          <a href="#" class="search"></a>
        </li>
      </ul>
    </div>
    <div class="navbar">
      <ul>
        <li>
          <a href="#">推荐</a>
        </li>
        <li>
          <a href="#">排行榜</a>
        </li>
        <li>
          <a href="#">搜索</a>
        </li>
      </ul>
    </div>
    <router-view></router-view>
  </div>
</template>

<script>
</script>

<style lang="scss">
html {
  font-size: 14px;
}
* {
  margin: 0px;
  padding: 0px;
}
.contain {
  width: 100%;
  height: 100%;
}
.top {
  width: 100%;
  height: 40px;
  ul {
    display: flex;
    justify-content: space-between;
    li {
      list-style-type: none;
      a {
        color: black;
        font-size: 1.6rem;
        text-decoration: none;
        line-height: 40px;
        text-align: center;
      }
    }
  }
}
.person::before {
  content: "\E613";
}
.search::before {
  content: "\E624";
}
.navbar {
  width: 100%;
  height: 40px;
  ul {
    display: flex;
    li {
      height: 40px;
      flex: 1;
      list-style-type: none;
      text-align: center;
      line-height: 40px;
      a {
        color: black;
        font-size: 1.5rem;
        text-decoration: none;
      }
    }
  }
}
</style>
