<template>
    <div class="bg-success text-white pt-2 rounded">
    <div>
         <slot name="green"></slot>
    </div>

  
  
            
      
    </div>
</template>
<script>
export default {
    data:function()
    {
        return{
            nm:0
        }
    },
    props:
    {
        
    },
    methods:
    {
  

    }
}

 









</script>
<style scoped>
   div
{
    width: 100%;
    height: 200px;
    
    text-align: center;
}
</style>