<script setup>
import { ref } from "vue";

  const input1 = ref('')
  const input2 = ref('')


</script>



<template>
    <div>
      
        <form>
            <label for="input1">Name</label>
                <input type="text" id="input1" v-model="input1" placeholder="Enter Name"  >
         
                <label for="input2">Number</label>
                <input type="text" id="input2" v-model="input2" placeholder="Enter Your Momo Pin" >
                <button v-show="input1 ==='Nana' && input2 == '05974'"><RouterLink to="/NextView">Submit</RouterLink></button>
      </form>
       
    </div>

</template>

<style scoped>
 form{
    display: flex;
    flex-direction: column;
    gap: 10px;
 }
.sectionInput{
    
    display: flex;
    flex-direction: column;
    gap:3px;

}

label{
    color: #000;
    font-size: 10px;
    font-style: normal;
    font-weight: 500;
    line-height: normal;
    font-weight: bold;
}
 

input{
    padding: 5px;
    border-radius: 2px;
   border: 1px solid #D9D9D9;
   background: #FFF;
   max-width: 400px;
  width: 100%;
  max-height: 44px;
  height: 100%;
  flex-shrink: 0;
}

label{
    font-size: 18px;
}
</style>