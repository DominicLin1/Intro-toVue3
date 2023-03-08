<template>
  <CoolButton @click="test">Click Me</CoolButton>
  <CoolCard v-for="animal in animals" :key="animal.title" :animal="animal" />
  <!--  <h1>{{ student }}</h1>
  <ul>
    <li v-for="animal in animals" :key="animal">{{ animal }}</li>
  </ul>

  <select v-model="selected">
    <option>A</option>
    <option>B</option>
    <option>C</option>
  </select>
  <h1 v-if="selected === 'A'">You are correct</h1>
  <h1 v-else-if="selected === ''">Please Answer</h1>
  <h1 v-else>You are Wrong</h1>
  <h2 v-if="graduated">You have graduated</h2> -->
</template>
<script>
import CoolCard from "../components/CoolCard.vue";
import CoolButton from "../components/CoolButton.vue";
export default {
  components: {
    CoolCard,
    CoolButton,
  },
  data() {
    return {
      student: "Daria",
      animals: [
        { title: "cat", desc: "sneaky animal who poops in my house" },
        { title: "Boggy-Woggy", desc: "Stands too close to his teachers" },
      ],
      selected: "",
      graduated: false,
      // text: "",
    };
  },
  methods: {
    test: function () {
      console.log("This is a test");
    },
  },
};
</script>
<style scoped>
h1 {
  color: red;
}
</style>
