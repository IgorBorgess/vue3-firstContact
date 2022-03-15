<template>
    <h2>Form: </h2>
    <form action="" @submit="sendForm($event)">
        <div> <input type="text" v-model="name" /> </div>
        <div> <input type="text" v-model="email" /> </div>
        <div> <Submit /> </div>
    </form>
</template>

<script>
import InputText from "./form/InputText.vue"
import Submit from "./form/Submit.vue"

export default {
    name: "Form",
    components: {
        InputText,
        Submit
    },
    data() {
        return {
            name: "",
            email: ""
        }
    },
    methods: {
        sendForm(event) {
            event.preventDefault()

            const name = this.name
            const email = this.email
            console.log("Formulário enviado.")
            console.log("O nome é: " + name)
            console.log("O email é: " + email)

            // Asynchronous request (Ajax)!
            // Insert the data into the database!
        }
    }
}
</script>

<style scoped>

</style>