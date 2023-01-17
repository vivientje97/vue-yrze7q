<template>
  <vue-list-picker :left-items="leftItems" :right-items="rightItems" />
</template>

<script>
import VueListPicker from './components/VueListPicker.vue';

export default {
  name: 'App',
  components: {
    VueListPicker,
  },
  data() {
      const example1 = {
        key: 1,
        content: "Item 1",
      };
      const example2 = {
        key: 2,
        content: "Item 2",
      };
      const example3 = {
        key: 3,
        content: "Item 3",
      };
      const example4 = {
        key: 4,
        content: "Item 4",
      };

      const leftItems = [example1, example2];
      const rightItems = [example3, example4];

      return { leftItems, rightItems };
    },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
