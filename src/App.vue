<!--form data bind with script using two way binding (v-model)-->
<template>
<pre>{{JSON.stringify(value,null,2)}}</pre>
<div id="div1">
  <h1>Student Information</h1>
  <form action="">
    <label for="name"> name</label>
    <input type="text" id="name" v-model="value.name" placeholder="name"><br>
    <label for="class">class</label>
    <input type="number" id="class" placeholder="(1-12)" v-model="value.class"><br>
    <label for="address">address</label>
    <input type="text" id="address" v-model="value.address" placeholder="address"><br>
    <label for="mail">G-mail</label>
    <input type="text" id="mail" v-model="value.mail" placeholder="xyz@gmail.com"><br>
    <label for="hobby">hobby</label>
    <textarea name="hobby" id="hobby" v-model="value.hobby"></textarea>
    <button v-on:click="color-red">summit</button>
    </form>
    </div> 
    <div>
      <select name="" id="country" v-model="value.country">
        <option value=""> </option>
        <option value="nepal">nepal</option>
    <option value="china">china</option>
    <option value="india">india</option>
      </select>
    </div>
</template>

<script>


export default {
  name: 'App',
 data(){
   return{ 
 value:{
name:'',
class:'',
address:'',
mail:'',
hobby:'',
country:''
 }
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
#div1{
  position: relative;

}
label {
font-weight:bold ;
margin-bottom: 5px;

}
input + label{
  font-weight: bold;
  margin-bottom: 20px;
  display: inline-flex;
}
#country{
  padding: 0.5rem;
  margin: 15px;
  width: 21rem;
}

</style>