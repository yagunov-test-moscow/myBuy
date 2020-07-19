<template>
<div class="container">
    <li>
      <Todoitem
      v-for="todo of todos"
      :todo="todo"
      :key="todo.id"
      v-on:remove-todo="removeTodo"
      />
  </li>
</div>
  
</template>

<script>
import Todoitem from '@/components/Todoitem.vue'

export default {
    props: ['todos'],
    components: {Todoitem},
    methods: {
      removeTodo (id) {
        this.$emit('remove-Todo', id)
      }
    }
}
</script>

<style scoped>
li {
  list-style: none;
}

</style>