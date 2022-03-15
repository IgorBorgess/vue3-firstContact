<template>
    <div>
        <button @click="$emit('changeImage')">Change profile image</button>
        <button @click="$emit('revertChange')">Revert profile image</button>
    </div>
</template>

<script>
export default {
    name: "ChangeImage",
    emits: ["changeImage", "revertChange"]
}
</script>

<style>

</style>