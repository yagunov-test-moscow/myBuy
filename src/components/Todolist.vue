<template>
<div class="container">
    <li>
      <Todoitem
      v-for="todo of todos"
      :todo="todo"
      :key="todo.id"
      />
  </li>
</div>
  
</template>

<script>
import Todoitem from '@/components/Todoitem.vue'

export default {
    props: ['todos'],
    components: {Todoitem}
}
</script>

<style scoped>
li {
  list-style: none;
}

</style>