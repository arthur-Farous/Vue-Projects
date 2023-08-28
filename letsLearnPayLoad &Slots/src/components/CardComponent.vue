<script setup>
defineProps(['h2','h5','h1'])

</script>

<template>
    <div class="container">
        <div class=" card">
            <h1>{{ h2 }}</h1>
        <p>{{h5}}</p>
        <h1>{{ h1 }}</h1>
        <slot></slot>
        </div>
   </div>
  
</template>


<style>

.container{
    background-color:green;
    display: flex;
    
    justify-content: center;
    margin: auto 0;
    align-items: center;
    padding:10px;
    border-radius: 16px;
    gap: 20px;
}

.card{
    display: flex;
    flex-direction: column;
    justify-content:center ;
    margin: 0 auto;
    align-items: center;
    padding: 20px;
}

h2{
    font-size: 36px;
    color: #fff;
}
h1{
    font-size: 64px;
    color: #fff;
}

h5{
    font-size: 18px;
    color: #fff;
}
</style>