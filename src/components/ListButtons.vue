<script setup>
import ButtonComp from '../components/ButtonComp.vue'

</script>

<template>
    <div>

        <ButtonComp class="up">up</ButtonComp>
        <ButtonComp class="submit">submit</ButtonComp>
        <ButtonComp class="down">down</ButtonComp>
    </div>

</template>

<style scoped>
div {
    display: flex;
    flex-direction: row;
    width: 100%;
    height: 4em;
    justify-content: space-around;

}

.up {
    background-color: blue;
}

.submit {
    background-color: red;
    align-self: flex-end;
}

.down {
    background-color: green;
}
</style>
