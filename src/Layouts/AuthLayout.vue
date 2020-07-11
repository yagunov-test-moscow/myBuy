<template>
    <div class="bg empty-layout">
        <router-view />
    </div>
</template>

<script>


export default {
}
</script>

<style lang="scss">
.bg {
  position: absolute;
  left: 0;
  top: 0;
  right: 0;
  bottom: 0;
  padding: 3em 1em;
  box-shadow: 0 0 10px rgba(0,0,0,.5);
  background:linear-gradient(90deg,
    #105B63 20%,
    #FFFAD5 20%, #FFFAD5 40%,
    #FFD34E 40%, #FFD34E 60%,
    #DB9E36 60%, #DB9E36 80%,
    #BD4932 80%
    ) 0 0 / 100% .4em no-repeat,
    linear-gradient(-90deg,
    #105B63 20%,
    #FFFAD5 20%, #FFFAD5 40%,
    #FFD34E 40%, #FFD34E 60%,
    #DB9E36 60%, #DB9E36 80%,
    #BD4932 80%
    ) 0 100% / 100% .4em no-repeat;
}
</style>