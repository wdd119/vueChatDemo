<template>
    <div>
        <p>我是Apart</p>
        <!-- 类似anguar的ng-click，用于绑定事件监听 -->
        <a v-on:click="goPage">点我切换</a>
    </div>
</template>

<script>
export default {
  name: 'test',
  methods: { // methods参数用来声明组件下的方法
    goPage: function () {
      this.$router.push('/bb')
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
p {
  color: red;
}
div {
    width: 100%;
    height: 100px;
    background-color: green;
}
</style>