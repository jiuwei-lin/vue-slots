<template>
  <div id="app">
    <FormHelper>
      <h2 slot="title">{{ title }}</h2>
      <p slot="text">I am the paragraph text</p>

      <div slot="form-header">
        <h3>This is the title of the form</h3>
        <p>Information about the form</p>
      </div>
      <div slot="form-fields">
        <input type="text" placeholder="name" required />
        <input type="password" placeholder="password" required />
      </div>
      <div slot="form-controls">
        <button @click="handleSubmmit">Submmit</button>
      </div>
    </FormHelper>
  </div>
</template>

<script>
import FormHelper from "@/components/FormHelper.vue";

export default {
  name: "app",
  components: {
    FormHelper
  },
  data() {
    return {
      title: "I am the dynamic slot title"
    };
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
