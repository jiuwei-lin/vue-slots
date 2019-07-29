<template>
  <div class="form-helpher">
    <slot name="title"></slot>
    <h1>I am the form helper</h1>
    <slot name="text"></slot>

    <h1>Please fill out our form...</h1>
    <form action>
      <div id="form-header">
        <slot name="form-header"></slot>
      </div>
      <div id="form-fields">
        <slot name="form-fields"></slot>        
      </div>
      <div id="form-controls">
        <slot name="form-controls"></slot>                
      </div>
      <div id="userful-links">
        <ul>
          <li>
            <a href="#"></a>1
          </li>
          <li>
            <a href="#"></a>2
          </li>
          <li>
            <a href="#"></a>3
          </li>
          <li>
            <a href="#"></a>4
          </li>
        </ul>
      </div>
    </form>
  </div>
</template>

<script>
export default {
  name: "FormHelper",
  props: {}
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  color: red;
}
</style>
