<template>
  <section id="experience" class="content-section">
    <h2 class="section-title">Pengalaman & Pencapaian</h2>
    <div class="card">
      <h3 class="job-title">Android Developer</h3>
      <p class="company-name">BarcodeScanner & hibaru</p>
      <ul class="achievements-list">
        <li>Mengembangkan aplikasi Android untuk scan barcode dan streaming film/TV menggunakan <strong>Kotlin</strong>, <strong>Jetpack Compose</strong>, dan <strong>Gradle</strong>.</li>
        <li>Menerapkan arsitektur MVVM, integrasi API eksternal (TMDB), serta deployment ke Play Store.</li>
        <li>Mengoptimalkan performa aplikasi dan pengalaman pengguna.</li>
      </ul>
    </div>
    <div class="card">
      <h3 class="job-title">Backend & Web Developer</h3>
      <p class="company-name">JBB-Panel & ApiCmt</p>
      <ul class="achievements-list">
        <li>Membangun RESTful API dan web admin panel menggunakan <strong>Python Flask</strong> dan <strong>Vue.js</strong>.</li>
        <li>Mengintegrasikan database <strong>SQL Server</strong> untuk manajemen packing list dan barcode.</li>
        <li>Menerapkan autentikasi, batch data, dan analitik produksi pada panel admin.</li>
        <li>Mengotomasi deployment dan monitoring aplikasi backend.</li>
      </ul>
    </div>
  </section>
</template>

<style scoped>
.content-section {
  margin-bottom: 6rem;
  scroll-margin-top: 6rem;
}
.job-title {
  font-size: 1.25rem;
  font-weight: 600;
  color: white;
}
.company-name {
  font-size: 1.125rem;
  font-weight: 500;
  color: var(--accent-secondary);
  margin-bottom: 1.5rem;
}
.achievements-list {
  list-style-type: none;
  padding-left: 0;
  display: flex;
  flex-direction: column;
  gap: 1rem;
}
.achievements-list li {
  line-height: 1.6;
  color: var(--text-secondary);
  padding-left: 1.5rem;
  position: relative;
}
.achievements-list li::before {
  content: '✓';
  position: absolute;
  left: 0;
  color: var(--accent-primary);
}
.achievements-list li strong {
  color: var(--text-primary);
  font-weight: 600;
}
</style>
