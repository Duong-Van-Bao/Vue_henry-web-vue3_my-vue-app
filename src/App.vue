<template>
  <div id="app">
    <Header/>
    <Todos/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Todos from './components/Todos.vue'
export default {
  name: 'app', //name này tương expost để file khác import ra dùng 
  components:{Header,Todos}
}
</script>

<style lang="css" scoped>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
}
</style>