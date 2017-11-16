<template>
  <div class="today">
    <h1>{{ msg }}</h1>
    <h2>Hello World !</h2>
  </div>
</template>

<script>
export default {
  name: 'today',
  data () {
    return {
      msg: 'This is Today'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
div {
  width:100%;
  height:300px;
  border:1px solid;
  background-color:red;  
}
</style>
