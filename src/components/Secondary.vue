<template>
  <div class="secondary">
    <div class="search">
      <el-input placeholder="请输入内容" v-model="input" clearable> </el-input>
      <el-button type="primary" icon="el-icon-search">搜索</el-button>
    </div>
    <div class="class_type">
      <section class="widget">
        <h3 class="widget-title">分类</h3>
        <ul class="widget-list">
          <li>
            <a href="https://www.liwenzhou.com/categories/Development/"
              >Development(14)</a
            >
          </li>

          <li>
            <a href="https://www.liwenzhou.com/categories/Django/">Django(3)</a>
          </li>

          <li>
            <a href="https://www.liwenzhou.com/categories/Front-end/"
              >Front-end(1)</a
            >
          </li>

          <li>
            <a href="https://www.liwenzhou.com/categories/Golang/"
              >Golang(89)</a
            >
          </li>

          <li>
            <a href="https://www.liwenzhou.com/categories/JavaScript/"
              >JavaScript(1)</a
            >
          </li>

          <li>
            <a href="https://www.liwenzhou.com/categories/Python/"
              >Python(13)</a
            >
          </li>
        </ul>
      </section>

      <section class="widget">
        <h3 class="widget-title">标签</h3>
        <div class="tagcloud">
          <a href="https://www.liwenzhou.com/tags/Development/">Development</a>

          <a href="https://www.liwenzhou.com/tags/Django/">Django</a>

          <a href="https://www.liwenzhou.com/tags/Golang/">Golang</a>

          <a href="https://www.liwenzhou.com/tags/Python/">Python</a>

          <a href="https://www.liwenzhou.com/tags/about/">about</a>

          <a href="https://www.liwenzhou.com/tags/front-end/">front-end</a>
        </div>
      </section>

      <section class="widget">
        <h3 class="widget-title">友情链接</h3>
        <ul class="widget-list">
          <li>
            <a
              target="_blank"
              href="https://geektutu.com"
              title="致力于分享有趣的技术实践"
              >极客兔兔-有趣的技术实践</a
            >
          </li>

          <li>
            <a target="_blank" href="https://draveness.me/golang/" title="灯塔"
              >draveness-Go语言设计与实现</a
            >
          </li>

          <li>
            <a
              target="_blank"
              href="https://www.cnblogs.com/liwenzhou/"
              title="Python全栈之路"
              >Q1mi-Python全栈之路</a
            >
          </li>

          <li>
            <a
              target="_blank"
              href="https://www.cnblogs.com/zhaof"
              title="Python/Go语言之路"
              >赵凡的博客</a
            >
          </li>

          <li>
            <a
              target="_blank"
              href="http://resn.cnblogs.com/"
              title="R_e-博客园"
              >R_e-博客园</a
            >
          </li>

          <li>
            <a target="_blank" href="http://roddypy.com/" title="罗迪's Blog"
              >罗迪's Blog</a
            >
          </li>
        </ul>
      </section>
    </div>
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
  methods: {},
  // 生命周期 - 创建完成（可以访问当前this实例）
  created() {},
  // 生命周期 - 挂载完成（可以访问DOM元素）
  mounted() {},
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
.secondary {
  padding-left: 2%;
  width: calc(100% - 80%);
}
.search {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: flex-start;
  margin-top: 30px;
}
.search input {
  width: 100%;
  border-radius: 4px 0px 0px 4px !important;
  border-right: none;
}
.search button {
  border-radius: 0px 4px 4px 0px !important;
}
.widget {
  margin-bottom: 30px;
}
.widget-title {
  color: #6e7173;
  line-height: 2.7;
  margin-top: 0;
  font-size: 16px;
  border-bottom: 1px solid #ddd;
  display: block;
}
#response {
  margin-bottom: 0.8em;
}
.widget-list {
  list-style: none;
  padding: 0;
}
.widget-list li {
  margin: 10px 0;
  line-height: 1.5;
}
.widget-list li a {
  color: #6e7173;
}
.widget .tagcloud {
  margin-top: 10px;
  display: flex;
  flex-direction: row;
  justify-content: flex-start;
  align-items: flex-start;
  flex-wrap: wrap;
}
.widget .tagcloud a {
  line-height: 1.5;
  padding: 5px;
  color: #6e7173;
}
@media screen and (max-width: 1000px) {
  .secondary {
    display: none;
  }
}
</style>