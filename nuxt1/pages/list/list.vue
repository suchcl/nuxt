<template>
  <div class="news">
    <h3><nuxt-link to="/">返回首页</nuxt-link></h3>
    <h3>推荐新闻</h3>
    <ul class="list">
      <li v-for="item in newsList" :key="item.cms_id">
        <a :href="item.url" target="_blank">{{ item.title }}</a>
      </li>
    </ul>
  </div>
</template>

<script>
import data from "../../static/data/news.json";
export default {
  data() {
    return {
      newsList: data,
    };
  },
};
</script>
<style scoped>
ul,
li,
ol {
  list-style: none;
  padding: 0;
}
.list li {
  height: 32px;
  line-height: 32px;
  font-size: 14px;
}
</style>
