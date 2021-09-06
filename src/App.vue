<template>
  <div id="app">
    <div class="container">
      <div class="row">
        <div class="col-md-12 col-md-offset-3 mt-3">
          <button @click="selectedComponent='Green'" class="btn btn-success">Green</button>
          <button  @click="selectedComponent='Yellow'" class="btn btn-warning">Yellow</button>
          <button  @click="selectedComponent='Blue'" class="btn btn-primary">Blue</button>
          <hr class="bg-danger">
          <keep-alive>
            <component :is="selectedComponent">
              <h1 slot="green">Green Page</h1>
              <h1 slot="yellow">Yellow Page</h1>
              <h1 slot="blue">Blue Page</h1>

            </component>
          </keep-alive>
          
       

      </div>
    </div>
   
  </div>
    </div>
</template>

<script>
import Green from './components/Green.vue'
import Yellow from './components/Yellow.vue'
import Blue from './components/Blue.vue'

export default
{
components:
{
  Green,
  Yellow,
  Blue
},
data:function(){
  return{
  selectedComponent:"Green"
  }
}
}
</script>

<style>
</style>
