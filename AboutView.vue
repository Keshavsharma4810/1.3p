<template>
  <div>
    <header>
      <h1>About Me</h1>
    </header>
    <main>
      <section class="about-me">
        <h2>Who I Am</h2>
        <p>I am a passionate web developer with a creative mind and a keen eye for detail. My journey into the world of web development started when I built my first website at the age of 16, and I've been hooked ever since. I specialize in front-end development, creating user-friendly and visually appealing web experiences.</p>
      </section>
      <section class="skills">
        <h2>Skills</h2>
        <ul>
          <li>HTML5 &amp; CSS3</li>
          <li>JavaScript (ES6+)</li>
          <li>Vue.js &amp; React</li>
          <li>Responsive Web Design</li>
          <li>UI/UX Design</li>
          <li>Version Control (Git)</li>
        </ul>
      </section>
      <section class="experience">
        <h2>Work Experience</h2>
        <table>
          <thead>
            <tr>
              <th>Position</th>
              <th>Company</th>
              <th>Year</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>Front-end Developer</td>
              <td>ABC Web Solutions</td>
              <td>2020-2022</td>
            </tr>
            <tr>
              <td>UI/UX Designer</td>
              <td>XYZ Design Studio</td>
              <td>2018-2020</td>
            </tr>
          </tbody>
        </table>
      </section>
      <section class="contact-form">
        <h2>Contact Me</h2>
        <form>
          <div class="form-group">
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" required>
          </div>
          <div class="form-group">
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>
          </div>
          <div class="form-group">
            <label for="message">Message:</label>
            <textarea id="message" name="message" rows="4" required></textarea>
          </div>
          <button type="submit">Submit</button>
        </form>
      </section>
    </main>
  </div>
</template>

<script>
export default {
  name: "About",
};
</script>

<style scoped>
/* Specific styles for the about section */
.about-me {
  background-color: #f8f9fa; /* Light gray background */
  border-radius: 15px; /* Slightly rounded corners */
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1); /* Soft shadow */
  padding: 2rem;
}

.about-me h2 {
  font-size: 1.8rem; /* Larger heading size */
  margin-bottom: 1.5rem; /* Increased bottom margin */
  color: #007bff; /* Blue heading color */
}

.about-me p {
  font-size: 1.1rem; /* Increased text size */
  line-height: 1.6;
  color: #343a40; /* Darker text color */
}

.skills ul {
  list-style-type: square; /* Changed list style to square bullets */
  padding-left: 1.5rem; /* Increased left padding */
}

.skills li {
  font-size: 1.1rem;
  margin-top: 0.8rem; /* Increased top margin */
}

/* Table styles */
.experience {
  margin-top: 3rem; /* Increased top margin */
}

table {
  width: 100%;
  border-collapse: collapse;
  margin-top: 1.5rem;
}

table th,
table td {
  padding: 0.7rem; /* Increased padding */
  text-align: left;
  border-bottom: 1px solid #dee2e6; /* Lighter border color */
}

/* Form styles */
.contact-form {
  background-color: #ffffff; /* White background */
  border-radius: 15px; /* Slightly rounded corners */
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1); /* Soft shadow */
  padding: 2rem;
  margin-top: 3rem; /* Increased top margin */
}

.contact-form h2 {
  font-size: 1.8rem;
  margin-bottom: 1.5rem;
  color: #007bff;
}

.form-group {
  margin-bottom: 1.5rem; /* Increased bottom margin */
}

.form-group label {
  display: block;
  font-size: 1.2rem; /* Increased label size */
  margin-bottom: 0.7rem; /* Increased bottom margin */
  color: #343a40; /* Darker label color */
}

.form-group input[type="text"],
.form-group input[type="email"],
.form-group textarea {
  width: 100%;
  padding: 0.7rem; /* Increased padding */
  font-size: 1.1rem; /* Increased input text size */
  border: 1px solid #ced4da; /* Lighter border color */
  border-radius: 7px; /* Slightly rounded corners */
}

.form-group textarea {
  resize: vertical;
}

button[type="submit"] {
  background-color: #007bff;
  color: #ffffff;
  border: none;
  border-radius: 7px;
  padding: 0.7rem 1.2rem; /* Increased padding */
  font-size: 1.1rem;
  cursor: pointer;
  transition: background-color 0.3s ease; /* Smooth hover transition */
}

button[type="submit"]:hover {
  background-color: #0056b3; /* Darker blue on hover */
}
</style>