<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
import TheButton from './components/TheButton.vue'
import CardComponent from './components/CardComponent.vue';
import TheLayout from './components/TheLayout.vue'


 import { ref } from 'vue';
 const text = ref('')
 const yawa = ref('')
function showPayout(payLoad){
   text.value = payLoad 
}

function ShowPayout(payLoad){
   yawa.value = payLoad
}
</script>

<template>
  <h1>{{yawa}}</h1>
  <p>{{ text }}</p>
  <TheButton @yes ="ShowPayout" @no ="ShowPayout" /> 
   <!-- <div class="deals">
   <CardComponent   h2="Personal" h5="Special First packet for all"  h1="$8/month"/>
   <CardComponent><p> Don't miss class today</p></CardComponent>  
</div> 
 <div class="deals">
  <CardComponent h2="Personal" h5="Special First packet for all"  h1="$8/month" />
    <CardComponent><img src="./assets/Microsoft_icon.svg"/></CardComponent>
 </div> -->

 <TheLayout>
       <template #mobile>
        Hello,This is a trial version of my code.
       </template>
       <template #desktop>
        <div class="picture">
          <img src="./assets/Microsoft_icon.svg"/>
        </div>
       </template>
       <template #first_nav>
        See You soon
       </template>
 </TheLayout>
 
  
</template>

<style scoped>
.deals{
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  gap: 20px;
}

.picture{
  display: flex;
  justify-content: center;
  align-items: center;
}

















/* header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
} */
</style>
