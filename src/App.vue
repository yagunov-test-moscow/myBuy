<template>
  <div id="app">
    <component :is="layout">
    </component>
  </div>
</template>

<script>
import MainLayout from '@/layouts/MainLayout'
import AuthLayout from '@/layouts/AuthLayout'

export default {
  components: {
    MainLayout, AuthLayout
  },
  computed: {
    layout() {
      return (this.$route.meta.layout) + '-layout'
    }
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
