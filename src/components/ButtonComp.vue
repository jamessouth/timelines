<script setup>

// function cl(e){
//     console.log(e);
//     @click="cl"
// }
</script>

<template>


    <button >
        <slot></slot>
    </button>


</template>

<style scoped>
    button{
        min-width: 4em;
        height: 2em;
    }



</style>
