<template>
  <h1 v-if="graduated">Congrats!</h1>
  <h1 v-else>You'll get em next time</h1>
  <h1>{{ student }}</h1>
  <ul>
    <li v-for="animal in animals" :key="animal">{{ animal }}</li>
  </ul>
</template>
<script>
export default {
  data() {
    return {
      graduated: false,
      student: "Yifan",
      animals: ["pig", "cow", "ostrich", "Leon"],
    };
  },
};
</script>
