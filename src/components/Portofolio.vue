<template>
  <section id="portfolio" class="content-section">
    <h2 class="section-title">Portofolio & Proyek Unggulan</h2>
    <div class="portfolio-grid">
      <a href="https://github.com/cumis1324" target="_blank" rel="noopener noreferrer" class="portfolio-card">
        <div class="icon-container">
          <i class="fab fa-github"></i>
        </div>
        <h3 class="portfolio-title">Profil GitHub</h3>
        <p class="portfolio-description">Jelajahi proyek kode, kontribusi, dan eksplorasi teknis saya di profil GitHub.</p>
      </a>
      <a href="#" target="_blank" rel="noopener noreferrer" class="portfolio-card">
        <div class="icon-container">
          <i class="fab fa-google-play"></i>
        </div>
        <h3 class="portfolio-title">Aplikasi di Play Store</h3>
        <p class="portfolio-description">Lihat aplikasi yang telah saya bangun dan rilis. (Tautan ke aplikasi Anda)</p>
      </a>
    </div>
  </section>
</template>

<style scoped>
.content-section {
  margin-bottom: 6rem;
  scroll-margin-top: 6rem;
}
.portfolio-grid {
  display: grid;
  gap: 2rem;
}
@media (min-width: 768px) {
  .portfolio-grid {
    grid-template-columns: repeat(2, 1fr);
  }
}
.portfolio-card {
  /* Menggunakan class .card global */
  text-align: center;
  text-decoration: none;
  color: var(--text-primary);
}
.icon-container {
  font-size: 3rem;
  color: var(--accent-primary);
  margin-bottom: 1rem;
  transition: transform 0.3s;
}
.portfolio-card:hover .icon-container {
  transform: scale(1.1);
}
.portfolio-title {
  font-size: 1.25rem;
  font-weight: 600;
  color: white;
}
.portfolio-description {
  color: var(--text-secondary);
  margin-top: 0.5rem;
}
</style>