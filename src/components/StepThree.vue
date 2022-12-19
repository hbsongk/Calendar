<template>
  <div class="container">
    <header>STEP 3 스케줄</header>
    <div v-if="visible" class="calendar" />
    <button @click="popCalendar">confidential</button>
  </div>
</template>

<script>
export default {
  name: "StepThree",
  data: function () {
    return {
      visible: false,
    };
  },
  methods: {
    popCalendar() {
      this.visible = !this.visible;
    },
  },
};
</script>

<style scoped>
.container {
  position: relative;
  display: flex;
  align-items: center;
  flex-direction: column;
  align-content: center;
  width: 60vw;
  height: 95vh;
  border: solid;
}

header {
  display: flex;
  justify-content: center;
  align-items: center;
  color: white;
  width: 95%;
  height: 10vh;
  margin: 3%;
  border-radius: 10px;
  background-color: #e52b50;
}
.calendar {
  width: 80%;
  height: 80%;
  background-color: black;
}
button {
  position: absolute;
  border: none;
  bottom: 0;
  right: 2%;
  width: 8vw;
  height: 4vh;
  background-color: #e52b50;
  color: white;
  cursor: pointer;
}
</style>
