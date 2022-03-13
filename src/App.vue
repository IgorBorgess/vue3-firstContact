<template>
  <div>
    <p class="father-paragraph">The test is being: {{ testing }}</p>
    <Header />
    <FirstComponent />
    <LifeCycle />
    <Person />
  </div>
</template>

<script>
import FirstComponent from "./components/FirstComponent.vue"
import LifeCycle from "./components/LifeCycle.vue"
import Person from "./components/Person.vue"
import Header from "./components/Header.vue"

export default {
  name: "App",
  components: {
    FirstComponent,
    LifeCycle,
    Person,
    Header
    },
  data() {
    return {
      testing: "made"
    }
  }
}
</script>

<style>
  body {
    background-color: #333;
    color: #FFF;
  }

  a {
    color: red;
  }

  .test {
    background-color: #000;
  }
</style>