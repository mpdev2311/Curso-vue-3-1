<template>        
  <div>
        <img :src="avatar" :alt="descricao">
        <MudarImagem @mudar-imagem="trocarImagem" />       
  </div>
</template>
<script>
import MudarImagem from "../components/MudarImagem.vue"
export default {
    name: 'Picture',
    components: {       
        MudarImagem
    },
    data() {
        return {
         avatar: '/img/avatar.png',
         descricao:  'Marcos Paulo'
        }
    },
    methods: {
        trocarImagem() {
         this.avatar = "/img/avatar2.png"
        }
    },
}
</script>