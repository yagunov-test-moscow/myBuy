<template>
  <div>
    <!-- <i class="material-icons" style="font-size: 5rem; margin-top: 150px;">attach_file</i>
    <h2>Здесь будут ваши заметки</h2> -->
    <Todolist/>
  </div>
</template>

<script>
import Todolist from '@/components/Todolist.vue'

export default {
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
