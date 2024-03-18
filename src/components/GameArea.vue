<script setup>
import CardComp from '../components/CardComp.vue'


let msgs = ["aaa", "bbb", "ccc", "ddd", "eee", "fff", "ggg", "hhh", "iii"];

let newMsg = true;
</script>

<template>


    <ul>
        <CardComp :newmsg="newMsg" v-show="newMsg" msg="hello" />
        <CardComp v-for="(m, i) in msgs" :key="m+i" :msg="m" />
    </ul>

</template>

<style scoped>
ul {
    height: 100%;
    width: 96%;
    margin: auto;
    background-color: lightcoral;
    overflow-y: scroll;
}

</style>
