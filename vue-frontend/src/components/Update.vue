<template>
    <div>

        <Header/>
    <h1>
        Hello User, Welcome to the Update Restraunt page
    </h1>
</div>
</template>
<script>
import Header from '../components/Header.vue'
export default{
    name : 'Update',
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