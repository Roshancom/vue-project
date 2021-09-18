<!--method in vue-->
<template>

 <h1>{{add(3,5,1)}}</h1>
 <h3>{{mod_div(21)}}</h3>
</template>

<script>


export default {
  name: 'App',
 data(){
   return{ 
 }
 },
 methods: {
 add(a,b,c){
   return a+b+c
 },
 mod_div(a){
return a%2
 }
 }
 }

</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
