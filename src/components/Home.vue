<template>
  <div>
    <h1>Hello From Home Component</h1>
    <!--    <h1 v-if="show">Hello From Home Component 2</h1>-->
    <!--    <button v-on:click="display()">Toggle Element</button>-->
    <!--    <h2>{{ data }}</h2>-->
    <!--    <h2>{{ msg }}</h2>-->
    <!--    <button v-on:click="hello('hello call')">Call Hello Function</button>-->
    <h1>For loop</h1>
    <table border="1px">
      <tr>
        <td>Id</td>
        <td>Name</td>
        <td>Email Address</td>
      </tr>
      <tr v-for="user in users" :key="user.id">
        <td>{{user.id}}</td>
        <td>{{user.name}}</td>
        <td>{{user.email}}</td>
      </tr>
    </table>
      <h1>Home Component</h1>
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
    hello(data) {
      alert(data)
    },
    display() {
      this.show = !this.show
    }
  },
  data() {
    // return {show: true};
    return {
      users: [
        {id: 1, name: 'peter', email: 'peter@email.com'},
        {id: 2, name: 'Tony', email: 'Tony@email.com'},
        {id: 3, name: 'Pony', email: 'Pony@email.com'},
        {id: 4, name: 'Monty', email: 'Monty@email.com'},
      ]
    }
  }
}
</script>

<style scoped>
  div{
    background-color: #dde5ec;
    height: 500px;
  }
</style>