<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld :msg="count"/>
 
    <myButton :name="name" :contador="count"/>
    <button @click="incrementCont" > {{nombre}} </button>
  </div>
</template>

<script>

import HelloWorld from './components/HelloWorld.vue'
import myButton from './components/myButton.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    myButton
},
data: ()=>({

  count:10,
  name:"algo",
  nombre:"incrementar"
  

}
),
methods:{

  incrementCont(){
    this.count++
}

}

}
</script>

<style>

  #app{
    text-align: center;




  }

</style>