<template>
    <div>
        <h2>Description of the person: {{ name }}</h2>
        <Info />
        <Form />
    </div>
</template>

<script>
import Info from './Info.vue'
import Form from './Form.vue'
export default {
    name: "Pessoa",
    components: {
        Info,
        Form
    },
    data() {
        return {
            name: "Igor"
        }
    }
}
</script>

<style>

</style>