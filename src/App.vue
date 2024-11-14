<template>
  <div>
    <h1>Калькулятор</h1>
    <input v-model.number="a" placeholder="Введіть число A" />
    <input v-model.number="b" placeholder="Введіть число B" />
    <button @click="calculateSum">Обчислити суму</button>
    <p>Сума: {{ sum }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      a: 0,
      b: 0,
      sum: 0,
    };
  },
  methods: {
    calculateSum() {
      this.sum = this.a + this.b;
    },
  },
};
</script>
