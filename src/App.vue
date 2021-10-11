<template>
<img alt="Delicious Food's" src="./assets/rest.jpg" class="rest_logo">
<registration/>
</template>
     
<script>
//import HelloWorld from './components/HelloWorld.vue'
import registration from './components/registration.vue'

export default {
  name: 'App',
  components: {
    registration
  }
}   
</script>

<style>
.rest_logo {
  width:100px;
  display: block;
  margin-left: auto;
  margin-right: auto;
  margin-top: 30px;
}
.rest_form {
  width:100px;
  display: block;
  margin-left: auto;
  margin-right: auto;
}
.register_form input{
    display: block;
    width: 300px;
    height: 40px;
    padding-left: 20px;
    margin-left :auto;
    margin-bottom: 30px;
    margin-right: auto;
    border: 1px solid skyblue;
}
.register_button{
    width: 320px;
    height: 40px;
    border: 1px solid skyblue;
    background : skyblue;
    color : #fff;
    cursor: pointer;
    display: block;
    margin-left: auto;
    margin-right: auto;
    
}
</style>
