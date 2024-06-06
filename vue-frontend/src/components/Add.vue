<template>
    <div>

        <Header />
        <div class="mainDiv">

            <h1>
                Add Restraunt
            </h1>

            <div class="register">

                <input type="text" v-model="restraunt.name" name="name" placeholder="Enter name">
                <input type="text" v-model="restraunt.address" name="address" placeholder="Enter Address">
                <input type="text" v-model="restraunt.contact" name="contact" placeholder="Enter Contact">
                <button type="button" v-on:click="addRestraunt">Submit</button>
            </div>
        </div>
    </div>
</template>
<script>
import Header from '../components/Header.vue'
export default {
    name: 'Add',
    components: {
        Header
    },
    data() {
        return {
            restraunt: {

                name: '',
                address: '',
                contact: ''
            }
        }
    },
    methods: {
        addRestraunt() {
            console.log(this.restraunt)
        }
    },
}
</script>
<style>
h1 {
    text-align: center;
    margin: 50px 0;
}
</style>