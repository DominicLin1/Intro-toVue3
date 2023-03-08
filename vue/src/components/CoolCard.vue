<template>
  <div>
    <h2>{{ animal.title }}</h2>
    <p>{{ animal.desc }}</p>
  </div>
</template>

<script>
export default {
  name: "CoolCard",
  props: {
    animal: Object,
  },
};
</script>

<style scoped>
div {
  height: 500px;
  width: 300px;
  background-color: red;
  color: white;
}
</style>
