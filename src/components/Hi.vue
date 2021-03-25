<template >
  <h1 class="red">My name is {{name}} {{title}} my age is {{age }}</h1>

</template>
<script>
export default{
  name:'Hi',
  props:{
    name:String,
    title:String,
    age:String,
  }
}

</script>
