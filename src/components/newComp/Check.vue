<template>
    
    <input type="checkbox" value="Clear it" @click='callme'/>
    <label :class="{done}">{{tasks[0].name}} </label> <br>   
    <input type="checkbox" value="Clear it" @click='callme'/>
    <label :class="{done}">{{tasks[1].name}} </label> <br>
    <input type="checkbox" value="Clear it" @click='callme'/>
    <label :class="{done}">{{tasks[2].name}} </label> <br>    


</template>

<script>
export default {
    name:'Check',
    data(){
        return(
            {
                tasks:[
                    {name:"Go for gym"},
                    {name:"Practice vue js"},
                    {name:"Learn rails"},
                ],
                
                done:false
            }
           
        )
    },
    methods:
    {
        callme()
        {
           this.done=!this.done
        }
    }
}
</script>

<style scoped>
.done
{
    background-color: rgb(73, 255, 73);
    /* color: white; */
}
</style>