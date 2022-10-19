<template>
  <div>
    <h3>Example</h3>
    <hr />
    <form @submit.prevent="addSubject" class="inputform">
      <label>Enter new subject: </label>
      <input v-model="newSubject" type="text" />
      <button>Add Subject</button>
    </form>
    <hr />
    <ul>
      <li v-for="(subject, index) in allSubjects">
        {{ subject.content }}
        <button @click="removeSubject(index)">Delete</button>
      </li>
    </ul>
  </div>
</template>

<script>
import { ref } from 'vue';

export default {
  setup() {
    const newSubject = ref('');
    const allSubjects = ref([]);

    function addSubject() {
      allSubjects.value.push({ content: newSubject.value });
      newSubject.value = '';
      console.log(allSubjects.value);
    }
    function removeSubject(index) {
      allSubjects.value.splice(index, 1);
    }
    return {
      newSubject,
      addSubject,
      allSubjects,
      removeSubject,
    };
  },
  name: 'Example',
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
hr {
  margin-bottom: 20px;
}
.inputform {
  display: flex;
  justify-content: space-between;
}
ul li button {
  margin-left: 35px;
}
</style>
