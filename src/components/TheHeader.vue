<template>
<!-- computed -->
<div>
  {{ fullName }}
</div>

</template>
<script>

export default{
    name:'app',
    data(){
        return{
          user: {
            first_name: 'Daniel',
            Last_name: 'Cruz',
          }
          
        }

      },
      computed: {
        fullName() {
          return `${this.user.first_name} ${this.user.Last_name}`
        },
      
      }, 
      methods:{
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