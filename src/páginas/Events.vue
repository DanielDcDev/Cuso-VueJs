<template>
    <div>
    <button @click.once="onClick">
      Enviar
    </button>
  <br>
  <div
   @mouseover="onMouseOver"
   @mouseout="onMouseOut">
   mouse
  
  </div>
  
  <br><br>
  
        <form 
        action="https://google.com"
        @submit.prevent="onSubmit">
  <input 
        type="text"
        @keyup.enter="onkeyup"
        >
  
          <button type="submit">
            Google
          </button>
        </form>
  </div>
  </template>
  
  <script>
  
  export default{
      name:'app',
      data(){
          return{
            
          }
  
          },
          methods: {
            onClick(Sevt) {
              console.log('click ', Sevt);
            },
            onMouseOver(Sevt) {
              console.log('mouse over', Sevt);
            },
            onMouseOut(Sevt){
              console.log('mouse out', Sevt);
            },
            onSubmit(Sevt) {
              console.log('submit', Sevt);
            },
            onkeyup(Sevt) {
              console.log('submit',Sevt);
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
  
  