<template>
    <div>
        <button @click="primeiroEvento(), segundo(), terceiro()">Ativar multiplos enventos</button>

        <p>{{multiplos_Eventos}}</p>
    </div>
</template>

<script>
export default {
    name: 'MultiplosEventos',
    components:{

    },
    data() {
        return {
           multiplos_Eventos: '', 
        }
    },
    methods: {
        primeiroEvento(e){
            this.multiplos_Eventos = 'primeiro evento ativado'
        },
        segundo(e){
            setTimeout(()=>this.multiplos_Eventos = 'segundo evento',1000)
        } ,
        terceiro(e){
            setTimeout(()=>this.multiplos_Eventos = 'terceiro evento',2000)
        }
    },

}
</script>

<style scoped>

div{
    margin: 100px;
}

</style>