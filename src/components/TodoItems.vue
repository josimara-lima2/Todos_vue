<template>
    <div class="space-y-2">
        <TodoItem :todo="todo"
            v-for="todo in $store.state.todos" 
            :key="todo.id">
        </TodoItem>
 
      </div>
</template>


<script>
import TodoItem from './TodoItem.vue';
export default {
    components: { TodoItem }
}
</script>