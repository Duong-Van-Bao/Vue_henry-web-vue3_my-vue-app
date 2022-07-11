<template>
  <p class="todo-item is-complated">
      <input type="checkbox">
      {{todoProps.title}}
      <button class="del-btn">delete</button>
  </p>
</template>

<script>
    export default {
        name: 'TodoItem',
        props:['todoProps']
    }
</script>

<style lang="css" scoped>
.todo-item {
    background:#f4f4f4;
    padding: 10px;
    margin: 0;
    border-bottom: 1px solid #ccc;
}
 .is-complated {
    text-decoration: line-through;
 }
 .del-btn {
     background: #ff0000;
     color: #fff;
     border: none;
     cursor: pointer;
     float: right;
 }
</style>