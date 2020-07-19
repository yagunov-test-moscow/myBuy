<template>
 <div class="container">
   <form @submit.prevent="onSubmit">
    <nav class="N/A transparent">
        <div class="nav-wrapper">
            <a href="#" class="burger" @click.prevent="$emit('click')">
                <i class="material-icons">dehaze</i>
            </a>
            <input placeholder="Заметка..." id="first_name" type="text" class="validate" v-model="title">
            <button class="btn-flat" type="submit">
                <i class="material-icons">keyboard_return</i>
            </button>
        </div>
    </nav>
  </form>
 </div>
</template>


<script>
export default {
    data() {
        return {
            title: ''
        }
    },
    methods: {
        onSubmit () {
            if (this.title.trim()) {
                const newTodo = {
                    id: Date.now(),
                    title: this.title,
                    completed: false
                }
                this.$emit('addTodo', newTodo)
                this.title = ''
            }
        }
    }
}
</script>

<style scoped>
nav {
    border-radius: 10px;
}
.nav-wrapper {
    display: flex;
    justify-content: center;
    margin: 1rem;
    background-color: white;
    border-color: none;
}
.material-icons {
    color: grey;
}
.burger {
    margin-right: 10px;
}

</style>