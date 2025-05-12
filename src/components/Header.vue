<template>
  <header>
    <div class="logo-container">
      <img src="C:\Users\hyper\OneDrive\Desktop\ISS296\anything-is-possible\src\assets\medtech_logo-f.png" alt="Medtech Logo" />
      <div class="logo-text">
        <h2>SMU Connect</h2>
      </div>
    </div>
    <nav>
      <ul>
        <li><router-link to="/">Home</router-link></li>
        <li><router-link to="/clubs">Our Clubs</router-link></li>
        <li><router-link to="/member-login">Member Login</router-link></li>
        <li><router-link to="/admin-login">Admin Login</router-link></li>
      </ul>
    </nav>
  </header>
</template>


<script setup>
import { ref } from 'vue'
const showDropdown = ref(false)
</script>

<style scoped>
.site-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #f8f8f8;
  padding: 1rem 2rem;
  box-shadow: 0 2px 4px rgba(0,0,0,0.1);
}

.nav {
  display: flex;
  align-items: center;
  gap: 1rem;
}

a {
  text-decoration: none;
  color: #333;
}

.dropdown {
  position: relative;
}

.dropdown-button {
  background: none;
  border: none;
  cursor: pointer;
  font-weight: bold;
  color: #333;
}

.dropdown-menu {
  position: absolute;
  top: 120%;
  left: 0;
  background: white;
  border: 1px solid #ccc;
  padding: 0.5rem;
  display: flex;
  flex-direction: column;
  z-index: 10;
}

.dropdown-menu a {
  padding: 0.25rem 0;
  color: #333;
}

.dropdown-menu a:hover {
  background-color: #f0f0f0;
}
</style>
