<template>
  <div>
    <Header />
    <Pessoa />

    <primeiroComponente />

    <p>This is {{ test }}</p>

    <LifeCycle />

  </div>
</template>

<script>
import Header from "./components/Header.vue";
import primeiroComponente from "./components/primeiroComponente.vue";
import LifeCycle from "./components/LifeCycle.vue";
import Pessoa from "./components/Pessoa.vue";

export default {
  name: "App",
  components: {
    Header,
    primeiroComponente,
    LifeCycle,
    Pessoa,
  },
  data() {
    return {
      test: "Only test",
    };
  },
};
</script>
<!-- globla css -- maniula o css de forma global  -->
<style>
body {
  background-color: #333;
  color: #fff;
}
a {
  color: #fff;
}
</style>