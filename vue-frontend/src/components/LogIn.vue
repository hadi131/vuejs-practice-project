
	<template>
    <div class="mainDiv">

        <img class="logo" src="../assets/th.jpeg" alt="">
        <h1>
            LogIn
        </h1>
        <div class="register">
            <input type="text" v-model="email" placeholder="Enter Email">
            <input type="text" v-model="password" placeholder="Enter Password">
            <button v-on:click="login">LogIn</button>
            <p>If you don not have an account then <router-link to="/sign-up">SignUp</router-link></p>

        </div>
    </div>
</template>
<script>
export default {
    name: 'LogIn',
    data() {
        return {
            email: '',
            password: ''
        }
    },
    methods: {
        login() {
            console.log(this.email, this.password)
        }
    },
}
</script>