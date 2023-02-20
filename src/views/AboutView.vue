<template>
  <div>
    <h2>Class Attendance Form</h2>
    <form>
      <div>
        <label for="studentName">Student Name:</label>
        <input type="text" id="studentName" v-model="studentName">
      </div>
      <div>
        <label for="className">Class Name:</label>
        <input type="text" id="className" v-model="className">
      </div>
      <div>
        <label for="date">Date:</label>
        <input type="date" id="date" v-model="date">
      </div>
      <div>
        <label for="attendance">Attendance:</label>
        <select id="attendance" v-model="attendance">
          <option value="present">Present</option>
          <option value="absent">Absent</option>
          <option value="late">Late</option>
        </select>
      </div>
      <button @click.prevent="submitForm">Submit</button>
    </form>
  </div>
</template>

<script>
export default {
  data() {
    return {
      studentName: "",
      className: "",
      date: "",
      attendance: "present"
    };
  },
  methods: {
    submitForm() {
      // Code to submit form data goes here
    }
  }
};
</script>



