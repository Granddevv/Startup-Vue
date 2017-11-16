<template>
  <div class="post">
    <h1>{{ msg }}</h1>
    <PostInput />
    <PostList v-bind:todos="todos" />
  </div>
</template>

<script>
import PostList from '@/components/PostList';
import PostInput from '@/components/PostInput';
export default {
  name: 'post',
  data () {
    return {
      msg: "Today's List",
      todos:[
        {
          title:"today",
          content:"first",
          complete:false
        },
        {
          title:"tomorrow",
          content:"second",
          complete:false
        },
      ],
    }
  },
  components:{
    PostList,
    PostInput,
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
div {
  width: 100%;
  height: 300px;
  border: 1px solid;  
}
</style>
