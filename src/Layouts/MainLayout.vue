<template>
<div>
    <Navbar 
    @click="isOpen = !isOpen" 
    @addTodo="newTodo"
    />
    <Sidebar 
    v-model="isOpen"
    @click="isOpen = !isOpen"
    />
    <router-view/>
    <Bottombar/>
</div>
</template>

<script>
import Navbar from '@/components/Navbar.vue'
import Sidebar from '@/components/Sidebar.vue'
import Bottombar from '@/components/Bottombar.vue'


export default {
  data: () => ({
    isOpen: false
  }),
  components: {
    Navbar, Bottombar, Sidebar
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
@import '~materialize-css/dist/css/materialize.min.css'
</style>