<template>
  <h1>{{ student }}</h1>
  <ul>
    <li v-for="animal in animals" :key="animal">{{ animal }}</li>
  </ul>
</template>
<script>
export default {
  data() {
    return {
      student: "Daria",
      animals: ["pig", "cow", "zebra", "Bogdan"],
    };
  },
};
</script>
