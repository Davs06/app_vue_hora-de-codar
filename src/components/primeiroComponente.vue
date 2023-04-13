<template>
  <div>
    <h1>Hello guys!!</h1>

    <p>My name is {{ nome }}, and my job is {{ job }}</p>
  </div>
</template>

<script>
export default {
  name: "primeiroComponente",
  data() {
    return {
      nome: "Davs",
      job: 'Dev Front-End'
    };
  },
};
</script>