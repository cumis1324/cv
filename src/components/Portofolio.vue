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
      <div class="portfolio-card">
        <div class="icon-container">
          <i class="fas fa-barcode"></i>
        </div>
        <h3 class="portfolio-title">BarcodeScanner</h3>
        <p class="portfolio-description">
          Android app untuk scan barcode berbagai format.<br>
          <strong>Tech stack:</strong> Kotlin, Jetpack Compose, Gradle.<br>
          <strong>Fitur:</strong> Scan barcode, UI modern, integrasi kamera.
        </p>
      </div>
      <div class="portfolio-card">
        <div class="icon-container">
          <i class="fas fa-film"></i>
        </div>
        <h3 class="portfolio-title">hibaru</h3>
        <p class="portfolio-description">
          Aplikasi streaming film & TV berbasis Android.<br>
          <strong>Tech stack:</strong> Kotlin, Jetpack, Firebase.<br>
          <strong>Fitur:</strong> Streaming, TMDB API, autentikasi, UI responsif.
        </p>
      </div>
      <div class="portfolio-card">
        <div class="icon-container">
          <i class="fas fa-server"></i>
        </div>
        <h3 class="portfolio-title">JBB-Panel</h3>
        <p class="portfolio-description">
          Web admin panel untuk packing list dan barcode.<br>
          <strong>Tech stack:</strong> Python Flask, Vue.js, SQL Server.<br>
          <strong>Fitur:</strong> Manajemen data, analitik produksi, autentikasi, batch data.
        </p>
      </div>
      <div class="portfolio-card">
        <div class="icon-container">
          <i class="fas fa-network-wired"></i>
        </div>
        <h3 class="portfolio-title">ApiCmt</h3>
        <p class="portfolio-description">
          RESTful API untuk packing list dan barcode.<br>
          <strong>Tech stack:</strong> Python Flask.<br>
          <strong>Fitur:</strong> Batch insert/update/delete, integrasi produk, dokumentasi API.
        </p>
      </div>
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