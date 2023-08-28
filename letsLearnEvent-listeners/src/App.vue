<script setup>
import { ref } from 'vue'
import ButtonGroup from './components/ButtonGroup.vue'


function displayYes(){
    console.log('yes');
}

function displayNo(){
    console.log('no');
};
</script>


<template>
    <ButtonGroup @yes ="displayYes" @no ="displayNo" />
   
</template>



<style scoped>

</style>