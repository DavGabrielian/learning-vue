<template>
    <div>
        <button v-on:click="increment">Increment</button>
        <p>Counter: {{ couunter }}</p>
        <p>Clicks: {{ clicks }}</p>
    </div>
</template>

<script>
export default {
  name: 'Counter',
  data() {
    return {
      counter: 0,
      clicks: 0
    }
},
methods: {
    increment() {
        this.counter = this.counter + 2;
        this.clicks++
    }
}
}
</script>

<style>
    
</style>