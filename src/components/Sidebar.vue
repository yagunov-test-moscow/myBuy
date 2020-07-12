<template>
      <ul class="sidenav app-sidenav" :class="{open: value}">
        <a href="#" class="burger" @click.prevent="$emit('click')">
            <i class="material-icons" style="right: 50px;">arrow_back_ios</i>
        </a>
        <br>
        vdvd
      </ul>
</template>

<script>
export default {
      props: ['value']
}
</script>

<style>
.sidenav {
    
    background-color: white;
    color: grey;
    padding: 10px;
    box-shadow: 0 2px 2px 0 rgba(0,0,0,0.87),
                0 3px 1px -2px rgba(0,0,0,0.87), 
                0 1px 8px 0 rgba(0,0,0,0.9);
}
.app-sidenav{
      padding: 50px;
      position:absolute;
      top:64px;width:250px;
      transition:transform .3s;
      transition:transform .3s,-webkit-transform .3s;
      bottom:0!important;
      height:auto!important
      }
.app-sidenav.open{
      -webkit-transform:translateX(0);
      transform:translateX(0)
      }
</style>