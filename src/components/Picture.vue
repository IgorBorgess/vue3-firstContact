<template>
    <img v-bind:src="avatar" :alt="description">
    <ChangeImage @change-image="changeImage" @revert-change="revertChange" />
</template>

<script>
import ChangeImage from "./ChangeImage.vue"

export default {
    name: "Picture",
    components: {
        ChangeImage
    },
    data() {
        return {
            avatar: "/img/avatar.png",
            description: "Guy with a computer"
        }
    },
    methods: {
        changeImage() {
            this.avatar = "/img/avatar2.png"
        },
        revertChange() {
            this.avatar = "/img/avatar.png"
        }
    }
}

</script>

<style>

</style>