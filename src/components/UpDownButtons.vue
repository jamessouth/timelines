<script setup>
    import ButtonComp from '../components/ButtonComp.vue'

</script>

<template>
<div>

    <ButtonComp class="up">up</ButtonComp>
    <ButtonComp class="down">down</ButtonComp>
</div>

</template>

<style scoped>
    div{
        display: flex;
        flex-direction: row;
        width: 100%;
        height: 3em;
        justify-content: space-around;
        align-content: center;
        margin-bottom: 1em;
    }
    .up{
        background-color: blue;
    }
    .down{
        background-color: green;
    }


</style>
