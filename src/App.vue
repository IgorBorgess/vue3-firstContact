<template>
  <FirstComponent />
  <p>The test is being: {{ testing }}</p>
</template>

<script>
import FirstComponent from "./components/FirstComponent.vue"

export default {
  name: "App",
  components: {
    FirstComponent,
    },
  data() {
    return {
      testing: "made"
    }
  }
}
</script>

<style>

</style>