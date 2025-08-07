<template>
  <div id="app-wrapper">
    <Header />
    <main class="main-container">
      <Hero />
      <About />
      <Experience />
      <Skills />
      <Education />
      <Portfolio />
      <Contact />
    </main>
    <Footer />
  </div>
</template>

<script setup>
import Header from './components/Header.vue';
import Hero from './components/Hero.vue';
import About from './components/About.vue';
import Experience from './components/Experience.vue';
import Skills from './components/Skills.vue';
import Portfolio from './components/Portofolio.vue';
import Contact from './components/Contact.vue';
import Footer from './components/Footer.vue';
</script>

<style scoped>
.main-container {
  max-width: 1024px;
  margin: 0 auto;
  padding: 3rem 1.5rem;
}
</style>