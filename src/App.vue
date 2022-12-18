<template>
  <div id="app">
    <step-one />
    <step-two />
    <step-three />
  </div>
</template>

<script>
import StepOne from "./components/StepOne.vue";
import StepTwo from "./components/StepTwo.vue";
import StepThree from "./components/StepThree.vue";
export default {
  name: "App",
  components: {
    StepOne,
    StepTwo,
    StepThree,
  },
};
</script>

<style>
#app {
  display: flex;
}
*{
  font-weight:bold;
}
</style>
