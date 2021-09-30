<template>
  <div class="list">
    <article class="post">
      <header>
        <h1 class="post-title">
          <router-link
            :to="{ path: '/detaile', query: {id : '1'} }"
          >
            【置顶】Go语言学习之路/Go语言教程</router-link
          >
        </h1>
      </header>
      <date class="post-meta meta-date"> 2021年9月23日 </date>

      <div class="post-meta meta-category">
        |

        <a href="https://www.liwenzhou.com/categories/Golang" target="_blank"
          >Golang</a
        >
      </div>

      <div class="post-content">
        <p>《Go语言学习之路》博客目录。</p>

        <p>
          2015年底我因为工作原因接触到了Go语言，那时网上关于Go语言的学习资料不多，我就边学边记笔记，一直坚持到现在。我把自己学习Go语言的笔记发布出来是希望能给Go语言社区出一点绵薄之力，帮助更多的人加入Gopher大家庭。
        </p>
      </div>
      <p class="readmore clearfix">
        <a href="https://www.liwenzhou.com/posts/Go/golang-menu/">阅读全文</a>
      </p>
      <p style="border-bottom: 1px solid #eee"></p>
    </article>

    <article class="post">
      <header>
        <h1 class="post-title">
          <a
            href="https://www.liwenzhou.com/posts/Go/golang-menu/"
            title="【置顶】Go语言学习之路/Go语言教程"
            target="_blank"
            >Go语言学习之路/Go语言教程1111</a
          >
        </h1>
      </header>
      <date class="post-meta meta-date"> 2021年9月23日 </date>

      <div class="post-meta meta-category">
        |

        <a href="https://www.liwenzhou.com/categories/Golang" target="_blank"
          >Golang</a
        >
      </div>

      <div class="post-content">
        <p>《Go语言学习之路》博客目录。</p>

        <p>
          2015年底我因为工作原因接触到了Go语言，那时网上关于Go语言的学习资料不多，我就边学边记笔记，一直坚持到现在。我把自己学习Go语言的笔记发布出来是希望能给Go语言社区出一点绵薄之力，帮助更多的人加入Gopher大家庭。
        </p>
      </div>
      <p class="readmore clearfix">
        <a href="https://www.liwenzhou.com/posts/Go/golang-menu/">阅读全文</a>
      </p>
      <p style="border-bottom: 1px solid #eee"></p>
    </article>

    <el-pagination
      @current-change="changePage"
      background
      layout="prev, pager, next"
      :total="10"
    >
    </el-pagination>
  </div>
</template>

<script>
// 这里可以导入其他文件（比如：组件，工具js，第三方插件js，json文件，图片文件等等）
// import PageHeaderLayout from '@/layouts/PageHeaderLayout'
// import ApeDrawer from '@/components/ApeDrawer'
// import ModalDialog from '@/components/ModalDialog'
// import ApeUploader from '@/components/ApeUploader'
// import ApeEditor from '@/components/ApeEditor'
// import { mapGetters } from 'vuex'

export default {
  components: {
    // PageHeaderLayout,
    // ApeDrawer,
    // ModalDialog,
    // ApeUploader,
    // ApeEditor
  },
  // 定义属性
  data() {
    return {};
  },
  // 计算属性，会监听依赖属性值随之变化
  computed: {
    // ...mapGetters(['userPermissions','buttonType'])
  },
  // 监控data中的数据变化
  watch: {},
  // 方法集合
  methods: {
    changePage(res) {
      console.log(res);
    },
  },
  // 生命周期 - 创建完成（可以访问当前this实例）
  created() {},
  // 生命周期 - 挂载完成（可以访问DOM元素）
  mounted() {
    
  },
  beforeCreate() {}, // 生命周期 - 创建之前
  beforeMount() {}, // 生命周期 - 挂载之前
  beforeUpdate() {}, // 生命周期 - 更新之前
  updated() {}, // 生命周期 - 更新之后
  beforeDestroy() {}, // 生命周期 - 销毁之前
  destroyed() {}, // 生命周期 - 销毁完成
  activated() {}, // 如果页面有keep-alive缓存功能，这个函数会触发
};
</script>

<style>
.list {
  width: 80%;
  border-right: 1px solid #ddd;
  padding-right: 2%;
  min-height: 760px;
}

.post {
  padding: 25px 0 25px 0;
  height: auto;
  overflow: hidden;
}
.post-title {
  margin: 0;
  color: #555;
  text-align: left;
  /**font:bold 25px/1.1 "ff-tisa-web-pro", Cambria, "Times New Roman", Georgia, Times, sans-serif;**/
  font-size: 1.5em;
  font-weight: bold;
}
.post-title a,
.keyword {
  color: #555;
}
.post-meta {
  padding: 0;
  margin: 9px 0 0;
  color: #999;
  text-align: left;
  display: inline-block;
}
.meta-category a {
  position: relative;
  margin-left: 1.8em;
}
.meta-category a:before,
.meta-category a:after {
  content: "";
  margin-left: -1.5em;
  position: absolute;
}
.meta-category a:before {
  width: 18px;
  height: 12px;
  background: #0089e0;
  border-radius: 0 0 1px 1px;
  margin-top: 4px;
}
.meta-category a:after {
  width: 6px;
  height: 0;
  left: 3px;
  border-style: solid;
  border-color: transparent transparent #0089e0 transparent;
  border-width: 0 1px 2px 1px;
  background: transparent;
  margin-top: 2px;
}
.meta-tags {
  display: inline-block;
}
.meta-tags ul {
  list-style: none;
  padding: 0;
  margin: 0;
}
.meta-tags ul li,
.meta-tags ul a {
  float: left;
  height: 24px;
  line-height: 24px;
  font-size: 14px;
  position: relative;
  padding: 0.3em 0;
}
.meta-tags ul a {
  margin-left: 24px;
  padding: 0 10px 0 14px;
  background: #0089e0;
  color: #fff;
  text-decoration: none;
  border-radius: 2px;
}
.meta-tags ul a:before {
  content: "";
  float: left;
  position: absolute;
  top: 0;
  left: -7px;
  width: 0;
  height: 0;
  border-color: transparent #0089e0 transparent transparent;
  border-style: solid;
  border-width: 12px 12px 12px 0;
  transition: all 0.1s ease-in;
}
.meta-tags ul a:after {
  content: "";
  position: absolute;
  top: 10px;
  left: 0;
  float: left;
  width: 4px;
  height: 4px;
  border-radius: 2px;
  background: #fff;
  box-shadow: -1px -1px 2px #004977;
}
.meta-tags ul a:hover {
  background: #555;
}
.meta-tags ul a:hover:before {
  border-color: transparent #555 transparent transparent;
}
.post-content {
  font-size: 1em;
  line-height: 1.7;
  color: #444;
  padding-top: 27px;
}
.post-content h2,
.post-content h3,
.post-content h4,
.post-content h5,
.post-content h6 {
  color: #ba3925;
}
.readmore a {
  font-size: 14px;
  color: #444;
  margin: 10px 0;
  padding: 5px 10px;
  border: 1px solid #ddd;
  border-radius: 5px;
  float: right;
}
.readmore a:hover {
  background: #f8f8f8;
  border-bottom-color: #d26911;
}
.meta-category a {
  position: relative;
  margin-left: 1.8em;
  color: #6e7173 !important;
}
.el-pagination {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
}
@media screen and (max-width: 1000px) {
  .list {
    width: 100%;
    border-right: none !important;
    padding-right: 0%none !important;
    min-height: auto !important;
  }
}
</style>