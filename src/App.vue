<template>
  <div class="app-container">
    <nav class="navbar">
      <div class="logo">Digital Eye Strain</div>
      <div class="nav-links">
        <router-link to="/">Home</router-link>
        <router-link to="/timer">Eye Timer</router-link>
        <router-link to="/tips">Tips</router-link>
        <router-link to="/settings">Settings</router-link>
      </div>
    </nav>

    <main class="main-content">
      <router-view></router-view>
    </main>

    <footer class="footer">
      <p>Take care of your eyes! © {{ new Date().getFullYear() }}</p>
    </footer>
  </div>
</template>

<script setup>
// Using Vue 3 Composition API with <script setup>
// Component logic will be added here as needed
</script>

<style>
/* Reset and base styles */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
  line-height: 1.6;
  color: #2c3e50;
  background-color: #f5f5f5;
}

.app-container {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
}

/* Navbar styles */
.navbar {
  background-color: #ffffff;
  padding: 1rem 2rem;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  font-size: 1.5rem;
  font-weight: bold;
  color: #2c3e50;
}

.nav-links {
  display: flex;
  gap: 2rem;
}

.nav-links a {
  text-decoration: none;
  color: #2c3e50;
  font-weight: 500;
  transition: color 0.3s ease;
}

.nav-links a:hover {
  color: #42b983;
}

.nav-links a.router-link-active {
  color: #42b983;
}

/* Main content styles */
.main-content {
  flex: 1;
  padding: 2rem;
  max-width: 1200px;
  margin: 0 auto;
  width: 100%;
}

/* Footer styles */
.footer {
  background-color: #ffffff;
  padding: 1rem;
  text-align: center;
  box-shadow: 0 -2px 4px rgba(0, 0, 0, 0.1);
}

.footer p {
  color: #666;
  font-size: 0.9rem;
}

/* Responsive design */
@media (max-width: 768px) {
  .navbar {
    flex-direction: column;
    padding: 1rem;
  }

  .nav-links {
    margin-top: 1rem;
    gap: 1rem;
  }

  .main-content {
    padding: 1rem;
  }
}
</style> 