<!--method in vue-->
<template>
<h1 v-text="name"></h1>
<button v-on:click="name='hari neupane'">change name</button>
<h2>{{count}}</h2>
<ol>
<button v-on:click="count +=1">incriment</button>
<button v-on:click="count -=1">decriment</button>
</ol>
</template>

<script>


export default {
  name: 'App',
 data(){
   return{ 
 name:"roshan neupane",
 count:0,
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
