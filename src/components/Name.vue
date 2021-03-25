<template lang="html">
  <h1>{{ msg }}</h1>
  <h1>{{ rev }}</h1>
  <button v-on:click='reverseName'>Click to reverse</button>
</template>

<script>
export default {
  name:'Name',
  props:{
    msg:String
  },
  data:{
    rev:"Hello world"
  },
  methods:
  {
    reverseName()
    {
      this.rev=this.rev.split('').reverse().join('')
      // alert('hi')
    }
  }
}
</script>

<style lang="css" scoped>
</style>
