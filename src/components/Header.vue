<template>
  <header class="header">
    <nav class="nav-container">
      <div class="logo">
        Hadyan<span class="accent-dot"> Jazila S.</span>
      </div>
      <div class="nav-links">
        <a v-for="link in navLinks" :key="link.href" :href="link.href">{{ link.title }}</a>
      </div>
      <div class="mobile-menu-button">
        <button @click="isMenuOpen = !isMenuOpen">
          <i class="fas fa-bars fa-lg"></i>
        </button>
      </div>
    </nav>
    <div class="mobile-menu" :class="{ 'is-open': isMenuOpen }">
      <a v-for="link in navLinks" :key="link.href" :href="link.href" @click="isMenuOpen = false">{{ link.title }}</a>
    </div>
  </header>
</template>

<script setup>
import { ref } from 'vue';
const isMenuOpen = ref(false);
const navLinks = [
  { href: '#about', title: 'About' },
  { href: '#experience', title: 'Experience' },
  { href: '#skills', title: 'Skills' },
  { href: '#portfolio', title: 'Portfolio' },
  { href: '#contact', title: 'Contact' },
];
</script>

<style scoped>
.header {
  background: rgba(10, 15, 31, 0.8);
  backdrop-filter: blur(10px);
  -webkit-backdrop-filter: blur(10px);
  position: sticky;
  top: 0;
  z-index: 50;
  border-bottom: 1px solid var(--border-color);
}
.nav-container {
  max-width: 1024px;
  margin: 0 auto;
  padding: 1rem 1.5rem;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.logo {
  font-size: 1.75rem;
  font-weight: 800;
  color: white;
}
.accent-dot {
  color: var(--accent-primary);
}
.nav-links {
  display: none;
}
@media (min-width: 768px) {
  .nav-links {
    display: flex;
    gap: 2rem;
  }
}
.nav-links a {
  color: var(--text-primary);
  position: relative;
  text-decoration: none;
  transition: color 0.3s ease;
}
.nav-links a:hover {
  color: white;
}
.nav-links a::after {
  content: '';
  position: absolute;
  width: 100%;
  transform: scaleX(0);
  height: 2px;
  bottom: -5px;
  left: 0;
  background-color: var(--accent-primary);
  transform-origin: bottom right;
  transition: transform 0.25s ease-out;
}
.nav-links a:hover::after {
  transform: scaleX(1);
  transform-origin: bottom left;
}
.mobile-menu-button {
  display: block;
}
@media (min-width: 768px) {
  .mobile-menu-button {
    display: none;
  }
}
.mobile-menu-button button {
  background: none;
  border: none;
  cursor: pointer;
  color: var(--text-primary);
}
.mobile-menu {
  display: none;
  background: rgba(10, 15, 31, 0.95);
}
.mobile-menu.is-open {
  display: block;
}
.mobile-menu a {
  display: block;
  padding: 1rem 1.5rem;
  font-size: 1rem;
  color: var(--text-primary);
  text-decoration: none;
  border-top: 1px solid var(--border-color);
}
.mobile-menu a:hover {
  background-color: var(--bg-card);
  color: white;
}
</style>
