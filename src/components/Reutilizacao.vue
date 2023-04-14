<template>
  <div>
    <button @click="ativar">Clique aqui</button>

    <span v-show="ativou">Ativado</span>
  </div>
</template>

<script>
export default {
  name: "Reutilizacao",

  data() {
    return {
      ativou: false,
    };
  },

  methods: {
    ativar(){
        if (!this.ativou){
            this.ativou = !this.ativou
        }else{
            this.ativou = !this.ativou
        }
    }
  },
};
</script>

<style scoped>
div {
  margin: 0 100px;
}
</style>