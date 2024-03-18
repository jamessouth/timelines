<script setup>
defineProps({
  msg: {
    type: String,
    required: true
  },
  newmsg: {
    type: Boolean,
    required: false
  }
})

</script>

<template>


   <li><div :class="{ red: newmsg }"><p>{{ msg }}</p></div></li>


</template>

<style scoped>
    li{
        border-top: 1px solid black;
        border-bottom: 1px solid black;
    }
    li:first-of-type{
        border-top: 2px solid black;
    }
    li:last-of-type{
        border-bottom: 2px solid black;
    }
    div{
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        background-color: lightgoldenrodyellow;
        height: 3em;
    }
    .red{
        background-color: red;
    }



</style>
