<template>
  <div>
    <primeiroComponente />
    <p> This is {{ test }}</p>
  </div>
</template>

<script>
import primeiroComponente from "./components/primeiroComponente.vue";

export default {
  name: "App",
  components: {
    primeiroComponente,
  },
  data() {
    return {
      test: 'Only test',
    }
  },
};
</script>