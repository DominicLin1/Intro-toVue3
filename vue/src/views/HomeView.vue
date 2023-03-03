<template>
  <h1 v-if="selected === 'A'">Wrong</h1>
  <h1 v-else-if="selected === 'B'">Wronger</h1>
  <h1 v-else-if="selected === 'C'">Right</h1>
  <h1 v-else="selected === ''">Answer A,B,C</h1>
  <h1>{{ student }}</h1>
  <ul>
    <li v-for="animal in animals" :key="animal">{{ animal }}</li>
  </ul>
  <select v-model="selected">
    <option>A</option>
    <option>B</option>
    <option>C</option>
  </select>
  <h2>{{ selected }}</h2>
</template>
<script>
export default {
  data() {
    return {
      graduated: false,
      student: "Yifan",
      animals: ["pig", "cow", "ostrich", "Leon"],
      text: "",
      selected: "",
    };
  },
};
</script>
