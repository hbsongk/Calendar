<template>
  <div class="container">
    <header>STEP 1 생산계획</header>
    <div class="order">
      <div class="column">회사명</div>
      <div class="column">모델명&REV</div>
      <div class="column">수량</div>
    </div>
    <div class="model" v-for="(item, index) in models" :key="index">
      {{ index + 1 }} {{ item }}
    </div>
  </div>
</template>

<script>
export default {
  name: "StepOne",
  data: function () {
    return {
      models: [
        "MCT_1호기",
        "MCT_2호기",
        "MCT_-------",
        "CNC_1호기",
        "CNC_2호기",
        "CNC_-------",
      ],
    };
  },
};
</script>

<style scoped>
.container {
  display: flex;
  align-items: center;
  flex-direction: column;
  align-content: center;
  width: 20vw;
  height: 95vh;
  border: solid;
}
.order {
  display: flex;
  justify-content: space-between;
  align-items: center;
  color: white;
  width: 90%;
  height: 10vh;
  margin: 2%;
}
.column {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 30%;
  height: 10vh;
  border-radius: 10px;
  background-color: #72a0c1;
}
header {
  display: flex;
  justify-content: center;
  align-items: center;
  color: white;
  width: 90%;
  height: 10vh;
  margin: 3%;
  border-radius: 10px;
  background-color: #e52b50;
}
.model {
  display: flex;
  justify-content: center;
  align-items: center;
  color: white;
  background-color: #007fff;
  width: 90%;
  height: 8vh;
  margin: 2%;
  border-radius: 10px;
}
</style>
