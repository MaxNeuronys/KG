<template>
<div class="board">
    <h1>Liste de mes postits</h1>
    <postits/>
</div>  
</template>
<script>
import postits from './postits.vue';
export default {
    name:"board",
    components: {
        postits
    }

}
</script>
<style scoped>
.board{
    height: 100vh;
    width: 100vw;
    background: grey;
    position:absolute;
    left: 0;
    right: 0;
    top: 0;
    margin: 0 auto;
    text-align: center;
    color: antiquewhite;
}
</style>