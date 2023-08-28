<script setup>
const emit = defineEmits(['yes','no']);

</script>

<template>

    <button @click="emit('yes','yes')" >yes</button>
    <button   @click="emit('no', 'no')" >no</button>
</template>