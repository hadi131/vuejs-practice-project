<template>
    <div class="navigation">
        <a href="#" v-on:click="Home">Home</a>
        <a href="#" v-on:click="Add">Add Restraunt</a>
        <a href="#" v-on:click="Update">Update Restraunt</a>
        <a href="#" v-on:click="logout">Logout</a>
    </div>
</template>
<script>
export default{
    name: 'Header',
    methods: {
        logout(){
            console.warn("Logged Out")
            this.$router.push({name:"LogIn"})
        },
        Add(){
            this.$router.push({name:"Add"})
        },
        Home(){
            this.$router.push({name:"Home"})
        },
        Update(){
            this.$router.push({name:"Update"})
        }
    },      
}
</script>


<style>
*{
    margin: 0;
    padding: 0;
}
.navigation{
    display: flex;
    justify-content: flex-start;
    align-items: center;
    background-color: rgb(42, 42, 42);
}
.navigation a{
    padding: 18px 23px;
    text-decoration: none;
    color: white;
}
.navigation a:hover{

    color: rgb(42, 42, 42);;
    background-color: white;
}
</style>