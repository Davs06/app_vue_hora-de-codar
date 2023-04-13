<template>
    <div>
        <h2>Meu nome é {{ name }}</h2>
        <INfoPessoa/>
        <Form/>
        <INfoPessoa/> <!-- Podese setar dados fiderentes do anterior-->
        <INfoPessoa/> <!-- Podese setar dados fiderentes do anterior-->
    </div>
</template>

<script>
import INfoPessoa from './INfoPessoa.vue'
import Form from './Form.vue';
export default {
    name: 'Pessoa',
    components: {
        INfoPessoa,
        Form
    },
    data() {
        return {
            name: 'Nelsão'
        }
    },
}
</script>