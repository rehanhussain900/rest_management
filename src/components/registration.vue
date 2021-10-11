<template>
    <div class="rest_form">
    <h1 class="">Sign Up </h1></div>
    <div class="register_form">
        
        <input type="text" v-model="name"  placeholder="Enter Name" />
        <input type="text" v-model="email" placeholder="Enter Email" />
        <input type="text" v-model="password" placeholder="Enter Password" />
        <button class="register_button" v-on:click="register">Sign Up</button>
    </div>
</template>
<script>
import axios from 'axios'

export default {
    name : 'registration',
    data(){
        return {
            name :'',
            email :'',
            password:''
        }
    },
    methods:{
      async  register(){
            
            let result = await axios.post("http://localhost:3000/users",{
                name:this.name,
                email:this.email,
                password:this.password
            });
            console.log(result);
            if(result.status =="201"){
                alert("Sign Up Successfully")
            }else{
                alert("Something Went Wrong")
            }
        }
    }
}

</script>
