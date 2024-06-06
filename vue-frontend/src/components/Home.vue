<template>
    <div>

        <Header/>
    <h1>
        Hello User, Welcome to the home page
    </h1>
</div>
</template>
<script>
import Header from '../components/Header.vue'
export default{
    name : 'Home',
    components:{
        Header
    }
}
</script>
<style>
h1{
    text-align: center;
}
</style>