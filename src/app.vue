<template>
  <div id="app">
    <div id="cover"></div>
    <App_Header></App_Header>
    <APP_Todo></APP_Todo>
  </div>
</template>


<script>
// 引入header.vue组件
import App_Header from './todo/header.vue';
// 引入todo.vue组件
import APP_Todo from './todo/todo.vue';

export default {
  components: {
    App_Header, APP_Todo
  },
  data () {
    return {
      text: 'abc223s'
    }
  }
}
</script>

<style scoped>
#app {
  position: absolute;
  left: 0;
  right: 0;
  top: 0;
  bottom: 0;
}
#cover {
  position: absolute;
  left: 0;
  right: 0;
  top: 0;
  bottom: 0;
  background-color: #555;
  opacity: 0.5;
  z-index: -1;
}
</style>
