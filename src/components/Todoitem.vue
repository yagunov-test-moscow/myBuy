<template>
 <div class="row">
  <div class="card-panel teal">
   <label>
    <input type="checkbox"
    v-on:change="todo.completed = !todo.completed"
    />
     <span style="font-size: 1.9rem; color: white;" class="check"></span>
    </label>
    <span class="white-text"
    :class="{done: todo.completed}"
    >{{todo.title}}
    </span>
    <a class="waves-effect waves-teal btn-flat"><i class="material-icons" style="font-size: 1.9rem; color: white;">delete_forever</i></a>
  </div>
 </div>
</template>

<script>
export default {
  props: {
    todo: {
      type: Object,
      required: true
    }
  }
}
</script>

<style scoped>
.card-panel {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 15px;
  margin-bottom: 0;
}
.btn {
  margin-left: 5px;
  overflow: inherit;
}
span.check::before{
  border-color: white;
}
[type="checkbox"]:checked+span:not(.lever):before{
    border-right: 2px solid white;
    border-bottom: 2px solid white;
}
.done {
  text-decoration: line-through;
  text-decoration-color: #000;
}

</style>