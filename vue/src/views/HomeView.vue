<template>
  <h1>{{ student }}</h1>
  <ul>
    <li v-for="animal in animals" :key="animal">{{ animal }}</li>
  </ul>
  <!-- <input v-model="text" />
  <p>{{ text }}</p> -->
  <select v-model="selected">
    <option>A</option>
    <option>B</option>
    <option>C</option>
  </select>
  <h1 v-if="selected === 'A'">You are correct</h1>
  <h1 v-else-if="selected === ''">Please Answer</h1>
  <h1 v-else>You are Wrong</h1>
  <h2 v-if="graduated">You have graduated</h2>
</template>
<script>
export default {
  data() {
    return {
      student: "Daria",
      animals: ["pig", "cow", "zebra", "Bogdan"],
      selected: "",
      graduated: false,
      // text: "",
    };
  },
};
</script>
<style scoped>
h1 {
  color: red;
}
</style>
