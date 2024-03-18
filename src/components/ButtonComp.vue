<script setup>

function cl(e){
    console.log(e);
}
</script>

<template>


    <button @click="cl">
        <slot></slot>
    </button>


</template>

<style scoped>
    button{
        min-width: 4em;
        height: 2em;
    }



</style>
