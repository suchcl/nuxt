<template>
  <div>
    <Tutorial />
    <div class="msg">{{ msg }}</div>
    <h3>用户信息</h3>
    <div>姓名：{{ person.name }}</div>
    <p>年龄：{{ person.age }}</p>
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
