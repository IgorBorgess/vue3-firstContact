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
    this.lifeCycle()
    },
    mounted() {
        setTimeout(() => {
            this.name = "Igor"
        }, 4000)
    this.lifeCycle()
    },
    methods: {
        lifeCycle() {
            console.log("Executou.")
        }
    }
}
</script>

<style>

</style>