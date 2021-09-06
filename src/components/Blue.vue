<template>
<div class="bg-primary text-white pt-2 rounded">
<slot  name="blue"></slot>

</div>
</template>
<script>
export default
{
    data:
    function(){
        return       {
           
        }
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