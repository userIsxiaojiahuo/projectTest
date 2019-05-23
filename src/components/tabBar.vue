<template>
  <div class="footer">
    <ul>
      <li v-for="(item,index) in tab"><a href="javascript:;"><i class="iconfont"
             v-html="item.icon"></i><span>{{item.title}}</span></a></li>
    </ul>
  </div>
</template>
<script>
export default {
  name: "tabBar",
  data() {
    return {
      tab: [
        {
          icon: "&#xe659;",
          title: "我们"
        },
        {
          icon: "&#xe645;",
          title: "垃圾箱"
        },
        {
          icon: "&#xe63f;",
          title: "购物车"
        }
      ]
    };
  }
};
</script>
<style scoped>
.footer {
  width: 100%;
  height: 1rem;
  border: 1px solid wheat;
  position: fixed;
  left: 0;
  bottom: 0;
}
.footer > ul {
  width: 100%;
  height: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.footer > ul > li {
  width: 100%;
  height: 100%;
}
.footer > ul > li > a > i {
  font-size: 0.4rem;
}
.footer > ul > li > a {
  display: block;
  font-size: 0.3rem;
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  align-items: center;
}
</style>