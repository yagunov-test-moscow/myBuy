<template>
        <footer class="page-footer white">
            <div class="buttons-list">
                <a class="btn-flat">Все</a>
                <a class="btn-flat">Активные</a>
                <a class="btn-flat">Выполненные</a>
            </div>
        </footer>
</template>

<script>
export default {

}
</script>

<style>

.page-footer.white{
    position: fixed;
    bottom: 0;
    width: 100%;
    background-color: white;
    color: grey;
    padding: 10px;
    box-shadow: 0 2px 2px 0 rgba(0,0,0,0.87),
                0 3px 1px -2px rgba(0,0,0,0.87), 
                0 1px 8px 0 rgba(0,0,0,0.9);
}
.buttons-list {
    display: flex;
    justify-content: space-around;
}
.btn-small{
    height: 100%;
    color: grey;
}

</style>