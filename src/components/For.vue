<template>
    <h2>Hello {{ msg }}</h2>
    <table border="50px">
        <tr>
            <td>ID</td>
            <td>Name</td>
            <td>Title</td>
        </tr>
        <!-- use this directive v-for and it seems like it is for each loop where the users value get into the user variable -->
        <tr v-for="user in users" > 
            <td>{{user.id}}</td>
            <td>{{user.name}}</td>
            <td>{{user.title}}</td>
        </tr>
    </table>
</template>
<script>
export default 
{
    name:"For",
    props:{
        msg:String
    },
    data()
    {
        return(
            {
                users:[
                    {id:1,name:"Sourav",title:"Das"},
                    {id:2,name:"Rick ",title:"Grimes"},
                    {id:3,name:"Daryl",title:"Dixion"},
                ]
            }
        )
    }
    
}
</script>