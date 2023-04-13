<template>
    <div>
        <h2>Meu nome é {{ name }}</h2>
        <INfoPessoa/>
    </div>
</template>

<script>
import INfoPessoa from './INfoPessoa.vue'

export default {
    name: 'Pessoa',
    components: {
        INfoPessoa
    },
    data() {
        return {
            name: 'Nelsão'
        }
    },
}
</script>