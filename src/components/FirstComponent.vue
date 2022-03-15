<template>
    <div>
        <h1>Hello, Vue!</h1>
        <!-- <p>My name is {{ name }}, I'm working as a {{ profession }}</p> -->
        <MultEvent />
        <Reuse />
    </div>
</template>

<script>
import MultEvent from "./MultEvent.vue"
import Reuse from "./Reuse.vue"

export default {
    name: "FirstComponent",
    components: {
        MultEvent,
        Reuse
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