<template>
  <div>
    <form action="" @submit="enviarForm($event)">
      <input type="text" v-model="nome"><br>
      <input type="text" v-model="email"><br>
      <InputBtn /><br />
    </form>
  </div>
</template>

<script>
import InputText from "./form/InputText.vue";
import InputBtn from "./form/InputBtn.vue";

export default {
  name: "Form",
  components: {
    InputText,
    InputBtn,
  },

  data() {
    return {
        nome:'',
        email: ''
    }
  },
  methods: {
    enviarForm(e) {

        e.preventDefault();
        
        const nome = this.nome
        const email = this.email

      console.log(`O nome é: ${nome}`);
      console.log(`O email é: ${email}`);
    },
  },
};
</script>