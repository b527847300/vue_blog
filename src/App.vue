<template>
  <div id="app">
    <header id="header">
      <div class="site-name">
        <div id="logo">孙博岩的博客</div>
        <p class="description">个人博客，记录代码，记录生活！</p>
      </div>
      <div id="nav">
        <!-- <router-link to="/">Home</router-link> |
        <router-link to="/about">About</router-link> -->
        <router-link to="/">首页</router-link>
        <router-link to="/archives">归档</router-link>
        <router-link to="/about">关于</router-link>
      </div>
    </header>
    <router-view />
    <footer>
      Copyright @ websuda.cn All Rights Reserved 备案号：黑ICP备19005954号-1
    </footer>
  </div>
</template>

<style>
#app {
  max-width: 80%;
  margin: 0 auto;
}
#header {
  width: 100%;
  padding: 58px 0 0;
  text-align: left;
}
footer {
  text-align: center;
  color: #999;
  line-height: 40px;
}
#logo {
  font-size: 37.5px;
  font-weight: bold;
  color: #555;
}
.description {
  margin: 5px 0 5px 0;
  color: #999;
}
#nav {
  margin-top: 20px;
  width: 100%;
  border-bottom: 1px solid #ddd;
  height: 40px;
  display: flex;
  flex-direction: row;
  justify-content: flex-end;
  align-items: center;
  line-height: 40px;
}
#nav a {
  padding: 0 20px;
  color: #555;
}
.router-link-exact-active {
  border: 1px solid #ddd;
  border-bottom: none !important;
}
@media screen and (max-width: 1000px) {
  #app {
    max-width: 90%;
  }
}
</style>
