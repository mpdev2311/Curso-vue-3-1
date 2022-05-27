<template>        
   <div>
       <h2>Essa é a descrição da pessoa: {{ name }}</h2>
       <Info :email="email" :esta_trabalhando=false /> 
       <Form />               
   </div>
</template>
<script>
import Info from './Info.vue'
import Form from './Form.vue'
export default {
    name: 'Pessoa',
    components: {
       Info,
       Form
    },
    data() {
        return {
          name: 'Francisca',
          email: "MrcosPaulo2@email.com"  
        }
    },
}
</script>