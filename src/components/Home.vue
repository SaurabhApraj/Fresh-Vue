<template>
  <div>
    <h1>Home Components</h1>
    <Users />
    <Product />
    <Product />
  </div>
</template>

<script>
import Users from "./Users";
import Product from "./Products";
export default {
  name: "Home",
  components: { Users, Product }
};
</script>

<style>
div {
  background-color: #eaf5ff;
  padding: 10px;
}
</style>