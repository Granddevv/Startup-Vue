<template>
  <div id="app">
    <img src="./assets/logo.png">
    <PostNote />
    <MainPart />
    <TodayPost />

    // <router-view/>
  </div>
</template>

<script>
import HelloWorld from '@/components/HelloWorld'
import MainPart from '@/components/MainPart'
import PostNote from '@/components/PostNote'
import TodayPost from '@/components/TodayPost'

export default {
  name: 'app',
  components: {
    MainPart,
    PostNote,
    TodayPost,
    HelloWorld
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
