<template>
  <div>
    <p>Meu nome: {{ nome }}</p>
  </div>
</template>

<script>
export default {
  name: "LifeCycle",
  data() {
    return {
      nome: "N sei ainda u.u",
    };
  },
  created() {
    setTimeout(() => {
      this.nome = "Davs";
    },1000);
  },
  mounted() {
    setTimeout(() => {
      this.nome = "Taw";
    },2000);
  },
};
</script>