<template>
  <div>
    <!-- <i class="material-icons" style="font-size: 5rem; margin-top: 150px;">attach_file</i>
    <h2>Здесь будут ваши заметки</h2> -->
    <Todolist 
    :todos="todos"
    @remove-Todo="removeTodo"
    />
  </div>
</template>

<script>
import Todolist from '@/components/Todolist.vue'

export default {
  data() {
    return {
      todos: [
      {id: 1, title: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit', completed: false},
      {id: 2, title: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit', completed: false},
      {id: 3, title: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit', completed: false}
    ]
    }
  },
  methods: {
    removeTodo (id) {
      this.todos = this.todos.filter(t => t.id !== id)
    }
  },
  components: {Todolist}
}
</script>

<style scoped>
/* h2 {
  margin-top: 30px;
  color: grey;
  font-size: 1.7rem;
} */
</style>
