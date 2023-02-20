<template>
  <div>
    <h1>Welcome to Course Portal</h1>
    <p>
      You have been directed to a portal that allows you to manage your course attendances and find information about your courses and teachers.
    </p>
    <h2>Course Attendance</h2>
    <p>
      With our attendance management system, you can easily keep track of your course attendance records, view your attendance history, and get alerts for any missed classes.
    </p>
    <router-link to="/about" class="button">Manage Attendance</router-link>
    <h2>Course Syllabus</h2>
    <p>
      Our course syllabus portal provides you with access to detailed information about your courses, including course objectives, topics, and assessments.
    </p>
    <router-link to="/before-class" class="button">View Syllabus</router-link>
    <h2>Teacher Information</h2>
    <p>
      Our teacher information portal allows you to access information about your course instructors, including their professional backgrounds, research interests, and teaching experience.
    </p>
    <router-link to="/before-class" class="button">View Teachers</router-link>
  </div>
</template>

<script>
export default {
  name: "HomePage"
};
</script>

<style scoped>
.button {
  display: block;
  margin-top: 10px;
  padding: 10px;
  background-color: #007bff;
  color: #fff;
  text-decoration: none;
  border-radius: 5px;
  text-align: center;
  width: 150px;
  cursor: pointer;
}
</style>
