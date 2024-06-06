<template>
    <div class="mainDiv">

        <img class="logo" src="../assets/th.jpeg" alt="">
        <h1>
            SignUp
        </h1>
        <div class="register">
            <input type="text" placeholder="Enter Name">
            <input type="text" placeholder="Enter Email">
            <input type="text" placeholder="Enter Password">
            <button>SignUp</button>
            <p>If you already have an account then <router-link to="/log-in">LogIn</router-link></p>
        </div>
    </div>
</template>
<script>
export default {
    name: 'SignUp'
}
</script>
<style>
.mainDiv{
  display: flex;
  flex-direction: column;
  align-items: center;
}

.logo {
  width: 100px
}

.register {
  display: grid;
  grid-template-columns: 1fr;
}
.register input{
  width: 300px;
  height: 40px;
  padding-left: 20px;
  margin-bottom: 30px;
  border: 1px solid skyblue
}
.register button {
  width: 320px;
  height: 40px;
      border: 1px solid skyblue;
background:skyblue;
color: white;;
cursor: pointer;
}






</style>
