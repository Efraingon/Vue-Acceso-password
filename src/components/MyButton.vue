<template>
  <button :style="{background, color}" :disabled="disabled">
    Button
  </button>

</template>

<script>
import { String } from 'core-js';

    export default {
    name: 'MyButtonItem',
     props:{
            color:{
                type:String
            },
            background:{
                type:String
            },
            disable:{
                type:Boolean
            }

     }        
    }
</script>


<style scoped>
    button:disabled{
            opacity:0.5;
    }
    
    button{
        background: none;
        color: black;
        border: none;
        border-radius: 5px;
        padding: 10px 40px;
        font-size: 16px;
        cursor: pointer;
    }
    button:hover{
        filter: brightness(125%);
    }      

</style>
