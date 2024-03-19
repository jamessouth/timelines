<script setup>
import CardComp from '../components/CardComp.vue'


defineProps({
  msgs: {
    type: Array,
    required: true
  }
})


</script>

<template>


    <ul>
        <CardComp :newmsg="m.new" v-for="(m, i) in msgs" :key="m.msg+i" :msg="m.msg" />
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
