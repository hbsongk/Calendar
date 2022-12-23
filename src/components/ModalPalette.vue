<template>
  <div id="app">
    <modal-view v-if="isModalViewed" @close-modal="isModalViewed = false" />
    <button
      v-for="(items, index) in machines"
      v-bind:key="index"
      @click="isModalViewed = true"
    >
      {{ items.이름 }}
    </button>
  </div>
</template>

<script>
import ModalView from "./ModalView.vue";
export default {
  name: "ModalPalette",
  components: {
    ModalView,
  },
  data() {
    return {
      isModalViewed: false,
      machines: [
        {
          이름: "cnc_1",
          공정: "황삭",
          요일: "월요일",
          시작시간: "12:00",
          종료시간: "14:00",
        },
        {
          이름: "cnc_2",
          공정: "황삭",
          요일: "월요일",
          시작시간: "12:00",
          종료시간: "14:00",
        },
        {
          이름: "cnc_2",
          공정: "황삭",
          요일: "월요일",
          시작시간: "12:00",
          종료시간: "14:00",
        },
      ],
    };
  },
};
</script>

<style></style>
