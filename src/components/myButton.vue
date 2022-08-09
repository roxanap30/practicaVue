<template>
  <div class="botom">

    <button>{{name}} {{contador}}</button>
  
  </div>
</template>

<script>
export default {
  name: 'newButton',
  props: {
    name: String,
    contador:Number
  }

}
</script>

