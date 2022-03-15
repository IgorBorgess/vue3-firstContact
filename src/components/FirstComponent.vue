<template>
    <div>
        <h1>Hello, Vue!</h1>
        <!-- <p>My name is {{ name }}, I'm working as a {{ profession }}</p> -->
        <MultEvent />
    </div>
</template>

<script>
import MultEvent from "./MultEvent.vue"
export default {
    name: "FirstComponent",
    components: {
        MultEvent
    },
    data() {
        return {
            name: "Igor",
            profession: "Dev"
        }
    }
}
</script>

<style>

</style>