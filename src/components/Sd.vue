<template lang="html">
    <h3> I am learning {{lang}}</h3>
    <h2 v-if='show'>Show this</h2>
    <button v-on:click='showhide'>Click to toggle</button>
    <h2>{{msg}}</h2>
    <button v-on:click='reverseName'>Click to revres</button>
</template>

<script>
export default {
  name:'Sd',
  props:{
    lang:{
      type:String,
      default:'vue'
    }
  },
  data()
  {
     return(
     {
       show:true,
       msg:"Hello world"
     });
  },
  methods:
  {
    showhide()
    {
      this.show=!this.show
    },
    reverseName()
    {
      this.msg=this.msg.split('').reverse().join('')
    }
  }
}
</script>

<style lang="css" scoped>
</style>
