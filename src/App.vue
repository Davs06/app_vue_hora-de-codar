<template>
  <div>
    <primeiroComponente />
    <p> This is {{ test }}</p>

    <LifeCycle/>
  </div>
</template>

<script>
import primeiroComponente from "./components/primeiroComponente.vue";
import LifeCycle from './components/LifeCycle.vue';

export default {
  name: "App",
  components: {
    primeiroComponente,
    LifeCycle
  },
  data() {
    return {
      test: 'Only test',
    }
  },
};
</script>