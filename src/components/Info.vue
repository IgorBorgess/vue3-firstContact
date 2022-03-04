<template>
    <div>
        <h3 v-if="is_employed">I'm working at the moment.</h3>
        <h3 v-else>I'm unemployed at the moment.</h3>
        <h3>I'm accostumed to using the following technologies:</h3>
        <u>
            <li>HTML</li>
            <li>CSS</li>
            <li>Javascript</li>
            <li>Vue.js</li>
            <li>TailwindCSS</li>
        </u>
        <h3 v-show="show_email">Send a message to {{ email }}.</h3>
        <h3>Para acessar meu portfólio <a v-bind:href="my_link" target="_blank">basta clicar aqui!</a></h3>
        <Picture />
    </div>
</template>

<script>
import Picture from "./Picture.vue"
export default {
    name: "Info",
    components: {
        Picture
        },
    data() {
        return {
            is_employed: false,
            show_email: true,
            email: "testingemail@email.com",
            my_link: "https://google.com"
        }
    }
}
</script>

<style>

</style>