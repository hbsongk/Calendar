<template>
  <div>
    <div v-for="(items, index) in machines" v-bind:key="index" @click="popModal()">
      {{ items.이름 }}
    </div>
  </div>
</template>

<script>
export default {
  name: "ProcessModal",
  data() {
    return {
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
  methods: {
      popModal() {
        
    },
  },
};
</script>

<style scoped></style>
