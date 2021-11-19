<template>
  <div>
    <Tutorial />
    <div class="msg">{{ msg }}</div>
    <h3>用户信息</h3>
    <div>姓名：{{ person.name }}</div>
    <p>年龄：{{ person.age }}</p>
    <ul class="link">
      <li>
        <a href="/list/list">新闻列表</a>
      </li>
      <li>
        <nuxt-link to="/list/list">列表</nuxt-link>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      msg: "Nuxt.js第一个项目",
      person: {
        name: "Nicholas Zakas",
        age: 18,
      },
    };
  },
};
</script>

<style scoped>
ul,
ol,
li {
  list-style: none;
  line-height: 2;
}
a {
  text-decoration: none;
}
a:hover {
  text-decoration: underline;
}
</style>
