
  <template>
    <div class="container">
      <h2>Welcome to Course Portal</h2>
      <p>You have been directed to a portal that allows you to manage your course attendances and find information about your courses and teachers.</p>
      <div class="row">
        <div class="col">
          <h3>Course Attendance</h3>
          <p>With our attendance management system, you can easily keep track of your course attendance records, view your attendance history, and get alerts for any missed classes.</p>
          <router-link to="/attendance">Manage Attendance</router-link>
        </div>
        <div class="col">
          <h3>Course Syllabus</h3>
          <p>Our course syllabus portal provides you with access to detailed information about your courses, including course objectives, topics, and assessments.</p>
          <router-link to="/syllabus">View Syllabus</router-link>
        </div>
        <div class="col">
          <h3>Teacher Information</h3>
          <p>Our teacher information portal allows you to access information about your course instructors, including their professional backgrounds, research interests, and teaching experience.</p>
          <router-link to="/teachers">View Teachers</router-link>
        </div>
      </div>
    </div>
  </template>


<script>
export default {
  name: "HomePage"
};
</script>

<style scoped>
.container {
  margin: 50px;
}

.row {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.col {
  flex: 1;
  margin: 10px;
  padding: 20px;
  background-color: #f0f0f0;
  border-radius: 5px;
}

h2, h3 {
  margin: 0 0 10px 0;
}

p {
  margin: 0 0 20px 0;
}
</style>
