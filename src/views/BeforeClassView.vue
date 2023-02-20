<template>
    <div>
      <h2>Course Curriculum Form</h2>
      <form @submit.prevent="submitForm">
        <div>
          <label for="courseName">Course Name:</label>
          <input type="text" id="courseName" v-model="courseName">
        </div>
        <div>
          <label for="curriculum">Course Curriculum:</label>
          <textarea id="curriculum" v-model="curriculum"></textarea>
        </div>
        <div>
          <label for="interest">Are you interested in this course?</label>
          <input type="checkbox" id="interest" v-model="interest">
        </div>
        <div>
          <label for="question">Do you have any questions about this course?</label>
          <textarea id="question" v-model="question"></textarea>
        </div>
        <button type="submit">Submit</button>
      </form>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        courseName: "",
        curriculum: "",
        interest: false,
        question: ""
      };
    },
    methods: {
      submitForm() {
        console.log("Form submitted:", this.courseName, this.curriculum, this.interest, this.question);
      }
    }
  };
  </script>
  