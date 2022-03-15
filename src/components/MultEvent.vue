<template>
    <div>
        <button @click="first(txt1, $event), second(txt2, $event), third(event)">Activate multiple events</button>
        <p>{{multiple_events}}</p>
    </div>
</template>

<script>
export default {
    name: "MultipleEvents",
    data() {
        return {
            multiple_events: "",
            txt1: "First event activated!",
            txt2: "Second event activated!"
        }
    },
    methods: {
        first(txt, event) {
            this.multiple_events = txt
        },
        second(txt, event) {
            setTimeout(() => {this.multiple_events = txt}, 2000)
        },
        third (event) {
            setTimeout(() => {this.multiple_events = ""}, 4000)
        }
    }
}
</script>

<style scoped>
    div {
        margin: 10px;
    }
</style>