<template>
  <div id="app">
    <h1>sample</h1>
    {{message}}
    <input @input="onInput" />
    <br>
    {{message2}}
  </div>
</template>

<script>
export default {
  name: "App",
  data: () => ({
    message: "input",
    message2:""
  }),
  methods: {
    onInput(event) {
      const text = event.target.value;
      this.message2 = text;
    }
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
