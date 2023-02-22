<template>
  <nav>
    <div class="logo">
      <img src="./assets/logoS.png" alt="Logo">
      <h1>Course Portal</h1>
    </div>
    <ul>
      <li><router-link to="/">Home</router-link></li>
      <li><router-link to="/about">Course Attendance</router-link></li>
      <li><router-link to="/before-class">Course Syllabus</router-link></li>
      <li><router-link to="/teachers">Teacher Information</router-link></li>
      <li><router-link to="/contact">Contact Us</router-link></li>
      <li><router-link to="/profile">Login</router-link></li>
    </ul>
  </nav>
  <router-view/>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  
}

nav {
  background-color: #ff8400;
  color: #fff;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px;
}

.logo {
  display: flex;
  align-items: center;
}

.logo img {
  width: 50px;
  margin-right: 10px;
}

ul {
  list-style: none;
  margin: 0;
  padding: 0;
  display: flex;
}

li {
  margin-right: 10px;
}

a {
  color: #fff;
  text-decoration: none;
  padding: 10px;
  border-radius: 5px;
}

a:hover {
  background-color: #ff8c10;
}
</style>
