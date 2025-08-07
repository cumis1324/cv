<template>
  <section id="experience" class="content-section">
    <h2 class="section-title">Pengalaman & Pencapaian</h2>
    <div class="card">
      <h3 class="job-title">Android Developer</h3>
      <p class="company-name">Gelaskaca</p>
      <ul class="achievements-list">
        <li>Memimpin refaktorisasi arsitektur aplikasi lawas (MVVM, Retrofit, Room), berhasil <strong>mengurangi tingkat kerusakan sebesar 80%</strong> dan <strong>meningkatkan rating Play Store dari 2.5 menjadi 4.2 bintang</strong>.</li>
        <li>Mengembangkan dan meluncurkan 5+ fitur utama, yang diadopsi oleh lebih dari <strong>200.000 pengguna</strong> dalam tiga bulan pertama.</li>
        <li>Mengoptimalkan kinerja rendering daftar dengan menerapkan DiffUtil dan Paging 3, yang <strong>mengurangi waktu muat hingga 50%</strong> pada perangkat kelas bawah.</li>
        <li>Memprakarsai alur CI/CD menggunakan GitLab CI, <strong>mempercepat siklus rilis sebesar 40%</strong> dan mengurangi kesalahan penerapan secara signifikan.</li>
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
