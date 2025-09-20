<template>
  <section id="contact" class="content-section">
    <h2 class="section-title">Hubungi Saya</h2>
    <div class="card">
  <p class="contact-text">Saya terbuka untuk peluang dan kolaborasi baru di bidang pengembangan Android, backend (Flask), dan web (Vue.js). Mari terhubung.</p>
      <div class="social-links">
        <a href="https://www.linkedin.com/in/hadyanjazila/" target="_blank" rel="noopener noreferrer" class="social-button">
          <i class="fab fa-linkedin"></i>
          <span>LinkedIn</span>
        </a>
        <a href="https://github.com/cumis1324" target="_blank" rel="noopener noreferrer" class="social-button">
          <i class="fab fa-github"></i>
          <span>GitHub</span>
        </a>
        <a href="mailto:email@hadyanjazila.my.id" class="social-button">
          <i class="fas fa-envelope"></i>
          <span>Email</span>
        </a>
      </div>
      <p class="email-notice">email@hadyanjazila.my.id</p>
    </div>
  </section>
</template>

<style scoped>
.content-section {
  margin-bottom: 6rem;
  scroll-margin-top: 6rem;
}
.card {
  /* Menggunakan class .card global dari style.css */
  text-align: center;
  padding: 2.5rem 1.5rem;
}
.contact-text {
  color: var(--text-primary);
  font-size: 1.25rem;
  margin-bottom: 2.5rem;
}
.social-links {
  display: flex;
  justify-content: center;
  gap: 1.5rem;
  flex-wrap: wrap;
}
.social-button {
  display: flex;
  align-items: center;
  gap: 0.75rem;
  padding: 0.75rem 1.5rem;
  border: 1px solid var(--border-color);
  border-radius: 0.5rem;
  color: var(--text-primary);
  text-decoration: none;
  transition: all 0.3s ease;
}
.social-button:hover {
  background-color: var(--accent-primary);
  border-color: var(--accent-primary);
  color: var(--bg-dark);
  transform: translateY(-3px);
  box-shadow: 0 0 15px rgba(0, 246, 255, 0.3);
}
.social-button i {
  font-size: 1.5rem;
  transition: color 0.3s ease;
}
.social-button:hover i {
  color: var(--bg-dark);
}
.email-notice {
  margin-top: 2.5rem;
  font-size: 0.875rem;
  color: var(--text-secondary);
}
</style>
