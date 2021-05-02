<template>
  <label>ToggleButton: </label>
  <toggle-button
      id="toggle"
      :initial-value="false"
      @onChange="onToggleButtonChanged($event)"
  />
</template>

<script>
  import ToggleButton from './components/ToggleButton.vue'

  export default {
    name: 'App',
    components: {
      ToggleButton
    },

    methods: {
      onToggleButtonChanged(event) {
        console.log(`Received onChange event from child component: ${event}`);
      }
    },
  }
</script>

<style>

</style>
