<template>
    <h1>My name is: {{ name }}</h1>
</template>

<script>
export default {
    name: "LifeCycle",
    data() {
        return {
            name: "Don't know it yet"
        }
    },
    created() {
        setTimeout(() => {
            this.name = "Igão"
        }, 2000)
    },
    mounted() {
        setTimeout(() => {
            this.name = "Igor"
        }, 4000)
    }
}
</script>

<style>

</style>