<template>
    <TodoItem v-for="todo in todos" v-bind:key="todo.id" v-bind:todoProps="todo"/>
</template>

<script>
import { ref } from 'vue';
import TodoItem from './TodoItem.vue'
export default {
    name: 'Todos',
    components: {
      TodoItem
    },
    setup() {
        const todos = ref([
            {
                id: 1,
                title: 'Viec 1',
                complated: false
            },
            {
                id: 2,
                title: 'Viec 2',
                complated: false
            },
            {
                id: 3,
                title: 'Viec 3',
                complated: false
            }
        ]) //khai báo state
        
        return {
            todos //gọi state ra và dùng nó 
        }
    } 
}
</script>

<style lang="scss" scoped>

</style>