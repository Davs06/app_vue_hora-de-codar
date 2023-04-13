<template>
    <div>
        <form action="">
            <InputText/><br>
            <InputText/><br>
            <InputBtn/><br>
        </form>
    </div>
</template>

<script>
import InputText from './form/InputText.vue'
import InputBtn from './form/InputBtn.vue';

export default {
    name: 'Form',
    components: {
        InputText,
        InputBtn        
    }

}
</script>