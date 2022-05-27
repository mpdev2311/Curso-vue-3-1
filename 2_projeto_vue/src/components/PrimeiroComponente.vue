<template>
  <div>
    <Reutilizacao />
     <h1>Olá Vue!</h1> 
     <Reutilizacao />
   <p>Meu nome é: {{ name }}, e trabalho como {{ Profissão }}.</p>
    <MultiplosEventos /> 
    <Reutilizacao />   
    <Reutilizacao />   
    <Reutilizacao />   
    <Reutilizacao />   
    <Reutilizacao />   
    <Reutilizacao />   
 </div>   
</template>

<script>
import MultiplosEventos from '../components/MultiplosEventos.vue';
import Reutilizacao from './Reutilizacao.vue'

export default {
    name: 'PrimeiroComponente',
    components: {
      MultiplosEventos,
      Reutilizacao
    }, 
    data() {
     return {
      name: 'Marcos',  
      Profissão: "Programador" 
     }   
   }
}
</script>