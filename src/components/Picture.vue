<template>
    <img v-bind:src="avatar" :alt="description">
</template>

<script>
export default {
    name: "Picture",
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