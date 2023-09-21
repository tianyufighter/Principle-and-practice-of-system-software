<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  <img :src="person.headImage" alt="头像">
  <h1>姓名: {{person.name}}</h1>
  <h2>性别: {{person.gender}}</h2>
  <h2 style="color:blue">家庭住址: {{person.address}}</h2>
  <h2>学号: {{person.studentID}}</h2>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  },
  data() {
    return {
      person: {
        name: '张洪涛',
        headImage: require('./assets/head.jpg'),
        address: '四川省达州市',
        gender: '男',
        studentID: '2310273046'
      }
    }
  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
