<template>
<div class="container">
    <li>
      <Todoitem/>
  </li>
</div>
  
</template>

<script>
import Todoitem from '@/components/Todoitem.vue'

export default {
    components: {Todoitem}
}
</script>

<style scoped>
li {
  list-style: none;
}

</style>