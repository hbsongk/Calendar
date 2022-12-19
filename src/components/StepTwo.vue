<template>
  <div class="container">
    <header>STEP 2 공정수령</header>
    <div class="step">소재 입고</div>
    <div class="step">황삭 1</div>
    <div class="step">열처리_외주</div>
    <div class="step">건드릴</div>
    <div class="step">센터_1</div>
    <div class="step">정상</div>
    <div class="step">MCT_1</div>
    <div class="step">연마 / 도금 /포장</div>
  </div>
</template>

<script>
export default {
  name: "StepTwo",
};
</script>

<style scoped>
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
.container {
  display: flex;
  align-items: center;
  flex-direction: column;
  align-content: center;
  width: 20%;
  height: 95vh;
  border: solid;
}
.step {
  display: flex;
  justify-content: center;
  align-items: center;
  color: white;
  background-color: #1cac78;
  width: 90%;
  height: 8vh;
  margin: 2%;
  border-radius: 50px;
}
</style>
