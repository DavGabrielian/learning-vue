<template>
  <div>
    <input type="text" v-on:input="CssClass = $event.target.value">
    <p v-bind:class="CssClass"> class: {{CssClass}}</p>
  </div>
</template>

<script>

export default {
  name: 'CssClass',
  data() {
    return {
      CssClass: ""
    }
}
}
</script>

<style>
.red {
  width: 100%;
  height: 50px;
  background-color: red;
}
.blue {
  width: 100%;
  height: 50px;
  background-color: blue;
}
</style>
