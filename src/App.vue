<template>
  <div>
    Component
    -------------------------------------------------------------------

    <Header />

    Component
    -------------------------------------------------------------------

    <primeiroComponente />
    not Component
    -------------------------------------------------------------------

    <p>This is {{ test }}</p>

    Component
    -------------------------------------------------------------------

    <LifeCycle />

    Component
    ------------------------------------------------------------------- 
    <Pessoa />
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