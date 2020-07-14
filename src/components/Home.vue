<template>
  <div>
    <h1 v-if="show">Conditional Rendering if part</h1>
    <h1 v-else>Conditional Rendering else part</h1>
    <button v-on:click="display">Toggle Element</button>
  </div>
</template>

<script>
export default {
  name: "Home",
  props: {
    data: String,
    msg: String
  },
  data() {
    return { show: true };
  },
  methods: {
    display() {
      this.show = !this.show;
    }
  }
};
</script>