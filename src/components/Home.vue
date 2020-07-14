<template>
  <div>
    <h1>Hello from Home Components.</h1>
    <h2>{{data}}</h2>
    <h2>{{msg}}</h2>
    <button v-on:click="hello">onClick</button>
    <button v-on:mouseover="mouse">mouseOver</button>
  </div>
</template>

<script>
export default {
  name: "Home",
  props: {
    data: String,
    msg: String
  },
  methods: {
    hello() {
      alert("Vue");
    },
    mouse() {
      alert("Mouse over");
    }
  }
};
</script>