<template>
 <nav class="N/A transparent">
    <div class="nav-wrapper">
        <a href="#" class="burger">
            <i class="material-icons">dehaze</i>
        </a>
          <input placeholder="Заметка..." id="first_name" type="text" class="validate">
        <a href="#" class="btn-flat disabled">
            <i class="material-icons">keyboard_return</i>
        </a>
    </div>
  </nav>
</template>


<script>
export default {

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