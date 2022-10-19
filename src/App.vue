<template>
  <div id="app">
    <Header
      heading="HTL Wels / 5AHIT"
      subheading="JavaScript / DOM-Manipulation / Dynamic List"
    />
    <Main />
    <Example />
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Main from './components/Main.vue';
import Example from './components/Example.vue';

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Example,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
