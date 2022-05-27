<template>         
   <h1>Meu nome é: {{ name }}</h1>
</template>

<script>
export default {
    name: "LifeCle",
    data() {
       return {
           name: 'Ainda não sei'
       } 
    },
    created() {
        setTimeout(() => {
            this.name = 'Marcos paulo'
        }, 1000);  
        
        this.lifeCycle()
    },
    mounted() {
           setTimeout(() => {
            this.name = 'Ana Claudia'
        }, 2000);

        this.lifeCycle()
    },
    methods: {
       lifeCycle() {
           console.log("Executou");
       } 
    },
}
</script>