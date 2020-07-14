<template>
  <div>
    <h1>For Loop</h1>
    <table border="1">
      <tr>
        <td>Id</td>
        <td>Name</td>
        <td>Lastname</td>
      </tr>
      <tr v-for="user in users" :key="user.id">
        <td>{{user.id}}</td>
        <td>{{user.name}}</td>
        <td>{{user.lastname}}</td>
      </tr>
    </table>
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
    return {
      users: [
        { id: 1, name: "Jeff", lastname: "Bezos" },
        { id: 2, name: "Bill", lastname: "Gates" },
        { id: 3, name: "Bernard", lastname: "Arnault" },
        { id: 4, name: "Mark", lastname: "Zuckerberg" },
        { id: 5, name: "Larry", lastname: "Ellison" }
      ]
    };
  },
  methods: {
    display() {
      this.show = !this.show;
    }
  }
};
</script>