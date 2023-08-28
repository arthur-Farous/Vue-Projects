<script setup>
defineProps(['buttonText'])
const { emit } = defineEmits(['yes', 'no'])
// function displayYes( displayYes) {
//     emit('no')
// }
   
// function displayNo(displayNo ) {
//     emit('yes')
// }
</script>

<template>
    <div>
<ButtonGroup @click="emit('yes')" | buttonText = "Yes"/>
<ButtonGroup @click="emit('no')"  | buttonText = "No" />
</div>
</template>



<style scoped>

button{
    display: flex;
    margin: 0 auto;
    padding-left: 16px;
    align-items: center;
    justify-content: center;
    background-color: black;
}

</style>