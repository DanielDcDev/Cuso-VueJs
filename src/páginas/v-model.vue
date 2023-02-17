<template>
    <div>
      <div>
  
        One-Way data binding <br>
        Two-Way data binding<br>
        v-model => formularios
  
      </div><br>
      <label class="nome">
        nome
      </label><br>
      <input
      type="text"
      v-model="name"
      ><br>
      {{ name }}
  <br><br>
      <div>
        <label >Sports</label><br>
        <select v-model="sports">
        <option value="basquete">Basquete</option>
        <option value="voley">Voley</option>
        <option value="judo">Judo</option>
        <option value="boxe">Boxe</option>
        </select>
        <br>
        {{ sports }}
  
    </div>
  
    <div>
      <br><br>
      <label>NewsLetter</label><br>
      <input
      v-model="newsLetter" 
      type="radio"
      value="yes"> Yes
  
      <input 
      v-model="newsLetter" 
      type="radio"
      value="No"> No
      <br>
    </div>
    <br><br>
    <label>Contract</label><br>
      <input
      v-model="newsLetter" 
      type="checkbox"> 
        I accept the contract
        <br>
      {{ contract }}
      <div>
      <br><br>
      <label>Colors do you like</label><br>
      <input
      v-model="colors" 
      type='checkbox'
      value='branco'> branco
  <br>
      <input 
      v-model="colors" 
      type="checkbox"
      value="preto"> preto
      <br>
      {{ colors }}
    </div>
  
  
  
  
  
  
    </div>
  
  </template>
  
  <script>
  
  export default{
      name:'app',
      data(){
          return{
            name:'Daniel Cruz',
            sports:'basquete',
            newsLetter: 'No',
            contract: true,
            colors: ['preto'],
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