<template>
  <h1> Hello world !!</h1>
  <primeiroComponente/>
</template>

<script>
import primeiroComponente from './components/primeiroComponente.vue';

export default {
  name:'App',
  components: {
    primeiroComponente
  }
}
</script>