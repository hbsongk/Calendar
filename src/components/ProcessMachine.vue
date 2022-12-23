<template>
  <div class="container">
    <header>장비명</header>
    <div v-for="(items, index) in machines" v-bind:key="index">
      {{ items }}
    </div>
  </div>
</template>

<script>
export default {
  name: "ProcssMachine",
  data() {
    return {
      machines: ["MCT_1", "MCT_2", "MCT_3", "CNC_1", "CNC_2", "CNC_3"],
    };
  },
};
</script>

<style scoped>
header {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 8vw;
  height: 8vh;
  color: white;
  background-color: red;
  margin: 3px;
  border: solid;
  border-color: red;
}
.container > div {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 8vw;
  height: 8vh;
  color: white;
  background-color: black;
  margin: 6px 3px;
  border: solid;
  border-color: black;
}
</style>
