<template>
    <img v-bind:src="avatar" :alt="description">
    <Reuse />
</template>

<script>
import Reuse from "./Reuse.vue"

export default {
    name: "Picture",
    components: {
        Reuse
    },
    data() {
        return {
            avatar: "/img/avatar.png",
            description: "Guy with a computer"
        }
    }
}
</script>

<style>

</style>