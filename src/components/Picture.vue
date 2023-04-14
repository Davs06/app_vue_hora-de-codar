<template>
  <div>
    <img :src="avatar" :alt="alt" />
    <!-- usando v-bind de forma resumida = : scr/herf ....-->

    <Reutilizacao />
  </div>
</template>
  
  <script>
import Reutilizacao from "./Reutilizacao.vue";

export default {
  name: "Picture",
  components: {
    Reutilizacao,
  },
  data() {
    return {
      avatar: "/img/avatar.jpg",
      alt: "profile_photo",
    };
  },
};
</script>


<!-- scoped css -- manipula o estilo do componente -->

<style scoped>
img {
  width: 100px;
  border-radius: 100px;
}
</style>