<script setup>
import CardComp from '../components/CardComp.vue'


let msgs = ["aaa", "bbb", "ccc"];
</script>

<template>



    <ul>


        <CardComp v-for="m in msgs" :key="m" :msg="m" />
    </ul>





</template>

<style scoped>
ul {
    min-height: 100%;
}
</style>
