<template>
  <header>
    <h1>HTL Wels / {{msg}}</h1>
    <h2>JavaScript / DOM-Manipulation / Dynamic List</h2>
  </header>
</template>

<script>
export default {
  name: 'Header',
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
header {
  border-bottom: 1px solid black;
  margin-bottom: 5px;
  text-align: center;
}
h1 {
  font-size: 3em;
}
</style>