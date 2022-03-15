<template>
    <div>
        <button @click="activate">Click here</button>
        <span v-show="activated">Ativado</span>
    </div>
</template>

<script>
export default {
    name: "Reuse",
    data() {
        return {
            activated: false
        }
    },
    methods: {
        activate() {
            this.activated = !this.activated
        }
    }
}
</script>

<style>
    div {
        margin: 10px;
    }
    span {
        padding-left: 10px;
    }
</style>