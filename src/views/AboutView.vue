<template>
  <div class="user-input">
    <form @submit.prevent="submitForm">
      <label for="fname">enter your name too see contact details:</label><br>
      <input type="text" id="fname" v-model="fName"><br>
      <button type="submit">Submit</button>
    </form>

    <div v-if="showDiv">
      <h2>Hello, {{ fName }}!</h2> 
      <table>
        <thead>
          <tr>
            <th>Email</th>
            <th>School</th>
            <th>GitHub</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td><a href="mailto:predding@deakin.edu.au">predding@deakin.edu.au</a></td>
            <td>Deakin</td>
            <td><a href="https://github.com/reddy-p" target="_blank">GitHub Profile</a></td>
          </tr>
          <!-- Add more rows as needed -->
        </tbody>
      </table>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      fName: '',
      showDiv: false,
    };
  },
  methods: {
    submitForm() {
      this.showDiv = true;
    }
  },
};
</script>

<style scoped>
.user-input {
  max-width: 400px;
  margin: 0 auto;
  text-align: center;
}

td {
  padding: 0rem 2rem;
}

table {
  border: 1px solid #0073e6;
}
</style>
