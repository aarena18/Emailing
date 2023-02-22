<template>
  <div class="attendance-form">
    <h2 class="form-title">Class Attendance Form</h2>
    <form class="form-container">
      <div class="form-group">
        <label for="studentName" class="form-label">Student Name:</label>
        <input
          type="text"
          id="studentName"
          v-model="studentName"
          class="form-input"
        />
      </div>
      <div class="form-group">
        <label for="className" class="form-label">Class Name:</label>
        <input
          type="text"
          id="className"
          v-model="className"
          class="form-input"
        />
      </div>
      <div class="form-group">
        <label for="date" class="form-label">Date:</label>
        <input type="date" id="date" v-model="date" class="form-input" />
      </div>
      <div class="form-group">
        <label for="attendance" class="form-label">Attendance:</label>
        <select id="attendance" v-model="attendance" class="form-input">
          <option value="present">Present</option>
          <option value="absent">Absent</option>
          <option value="late">Late</option>
        </select>
      </div>
      <button @click.prevent="submitForm" class="form-button">Submit</button>
    </form>
  </div>
</template>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.attendance-form {
  margin: 20px;
  padding: 20px;
  border: 1px solid #ddd;
  border-radius: 5px;
  background-color: #fff;
  box-shadow: 0 2px 6px rgba(0, 0, 0, 0.1);
}

.form-title {
  font-size: 1.5rem;
  font-weight: bold;
  margin-bottom: 20px;
  color: #ff8400;
  text-align: center;
}

.form-container {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.form-group {
  margin-bottom: 15px;
  display: flex;
  align-items: center;
}

.form-label {
  font-size: 1.2rem;
  font-weight: bold;
  margin-right: 10px;
  color: #333;
  flex: 1;
}

.form-input {
  padding: 10px;
  font-size: 1rem;
  border: 1px solid #ddd;
  border-radius: 5px;
  box-sizing: border-box;
  flex: 2;
}

.input-small {
  width: 100%;
  max-width: 200px;
}

.input-large {
  width: 100%;
  max-width: 300px;
}

select.form-input {
  -webkit-appearance: none;
  -moz-appearance: none;
  appearance: none;
  padding: 10px 30px 10px 10px;
  background-position: right 10px center;
  background-size: auto 60%;
}

.form-button {
  background-color: #ff8400;
  color: #fff;
  border: none;
  padding: 10px 20px;
  font-size: 1.2rem;
  border-radius: 5px;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

.form-button:hover {
  background-color: #d46400;
}
</style>

<script>
export default {
  data() {
    return {
      studentName: "",
      className: "",
      date: "",
      attendance: "present",
    };
  },
  methods: {
    submitForm() {
      // Code to submit form data goes here
    },
  },
};
</script>
