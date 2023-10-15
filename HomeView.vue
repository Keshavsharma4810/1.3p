<template>
<div>
    <header>
      <h1>Welcome to My Portfolio</h1>
    </header>
    <main>
      <section class="intro">
        <h2>Hello, I'm Keshav</h2>
        <p>Welcome to my portfolio website. I'm a web developer passionate about creating user-friendly and visually appealing websites. Explore my projects below.</p>
      </section>
      <section class="featured-projects">
        <div class="project-card" v-for="project in projects" :key="project.id">
          <img :src="project.image" :alt="project.title">
          <h3>{{ project.title }}</h3>
          <p>{{ project.description }}</p>
        </div>
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
  name: "Home",
  data() {
    // Your data remains unchanged
  },
};
</script>

<style scoped>
/* Specific styles for the home page */
.intro {
  background-color: #ff69b4; /* Pink */
  border-radius: 15px; /* Increased border-radius */
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
  padding: 2rem;
  text-align: center;
}

.intro h2 {
  font-size: 2rem; /* Increased font size */
  margin-bottom: 1rem;
}

.intro p {
  font-size: 1.2rem; /* Increased font size */
  line-height: 1.6;
}

.featured-projects {
  margin-top: 3rem; /* Increased margin-top */
}

.project-card {
  background-color: #db7093; /* PaleVioletRed */
  border-radius: 15px; /* Increased border-radius */
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
  padding: 1.5rem;
  margin-bottom: 3rem; /* Increased margin-bottom */
  text-align: center;
}

.project-card img {
  max-width: 80%; /* Reduced image width */
  height: auto;
  margin-bottom: 1rem; /* Increased margin-bottom */
}

.project-card h3 {
  font-size: 1.8rem; /* Increased font size */
  margin-top: 1.5rem; /* Increased margin-top */
}

.project-card p {
  font-size: 1.4rem; /* Increased font size */
  margin-top: 1rem; /* Increased margin-top */
}

/* Form styles */
.contact-form {
  background-color: #ffffff; /* White */
  border-radius: 15px; /* Increased border-radius */
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
  padding: 2rem;
  margin-top: 3rem; /* Increased margin-top */
}

.contact-form h2 {
  font-size: 2rem; /* Increased font size */
  margin-bottom: 1.5rem; /* Increased margin-bottom */
}

.form-group {
  margin-bottom: 2rem; /* Increased margin-bottom */
}

.form-group label {
  display: block;
  font-size: 1.2rem; /* Increased font size */
  margin-bottom: 1rem; /* Increased margin-bottom */
}

.form-group input[type="text"],
.form-group input[type="email"],
.form-group textarea {
  width: calc(100% - 2rem); /* Adjusted width */
  padding: 1rem;
  font-size: 1.2rem; /* Increased font size */
  border: 1px solid #db7093; /* PaleVioletRed */
  border-radius: 10px; /* Increased border-radius */
}

.form-group textarea {
  resize: vertical;
}

button[type="submit"] {
  background-color: #4169e1; /* RoyalBlue */
  color: #ffffff;
  border: none;
  border-radius: 10px; /* Increased border-radius */
  padding: 1rem 2rem; /* Increased padding */
  font-size: 1.2rem; /* Increased font size */
  cursor: pointer;
  transition: background-color 0.3s ease;
}

button[type="submit"]:hover {
  background-color: #0000cd; /* MediumBlue */
}
</style>
