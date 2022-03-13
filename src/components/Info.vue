<template>
    <div>
        <h3 v-if="is_employed">I'm working at the moment.</h3>
        <h3 v-else>I'm unemployed at the moment.</h3>
        <h3>Backend technologies:</h3>
        <ul >
            <li v-for="(technology, index) in backend_technologies" v-bind:key="index">{{ technology }}</li>
        </ul>
        <p>Frontend technologies:</p>
        <ul>
            <li v-for="technology in frontend_technologies" v-bind:key="technology.id">{{ technology.language }}</li>
        </ul>
        <div>
            <button @click="showEmail">{{ buttonText }}</button>
        </div>
        <h3 v-show="show_email">Send a message to {{ email }}.</h3>
        <h3 class="test">To access my portfolio <a v-bind:href="my_link" target="_blank">click here!</a></h3>
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
            show_email: false,
            email: "testingemail@email.com",
            my_link: "https://google.com",
            buttonText: "Show e-mail",
            backend_technologies: ["NodeJS", "Java"],
            frontend_technologies: [
                {id: 1, language: "HTML"},
                {id: 2, language: "CSS"},
                {id: 3, language: "Vue"}
            ]
        }
    },
    methods: {
        showEmail() {
            this.show_email = !this.show_email
            if(!this.show_email) {
                this.buttonText = "Show e-mail"
            } else {
                this.buttonText = "Hidden e-mail"
            }
        }
    }
}
</script>

<style>
    .father-paragraph {
    color: red;
    }
</style>