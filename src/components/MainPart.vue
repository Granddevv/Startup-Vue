<template>
  <div class="MainPart">
    <h1>{{ msg }}</h1>
  </div>
</template>

<script>
export default {
  name: 'MainPart',
  data () {
    return {
      msg: 'This is Main Part'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
div {
  width:100%;
  height:300px;
  border: 1px solid;  
}
</style>
