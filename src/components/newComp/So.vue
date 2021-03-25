<template>
    <h2>Tasks</h2>
    <!-- <Check/> -->
    <h4>{{msg}}</h4>
    <input type="text" v-model="msg">
    <!-- <p v-html="html"></p> -->
    <!-- <button v-bind:disabled='disbtn'>Thanos</button>111 -->
</template>
<script>
import Check from './Check'
export default {
    name:'So',
    components:{
        Check
    },
    data()
    {
        return(
        {
            name:'Sourav',
            html:' <h1>  Your name</h1>',
            disbtn:false,
            msg:'This is data'
        }
        
        )
    }
}
</script>