<template>
  <section id="skills" class="content-section">
    <h2 class="section-title">Keahlian & Sertifikasi</h2>
    <div class="card">
      <div class="skills-block">
        <h3 class="sub-title">Keahlian Inti</h3>
        <div class="skills-container">
          <span v-for="skill in coreSkills" :key="skill" class="skill-badge">{{ skill }}</span>
        </div>
      </div>
      <div class="skills-block">
        <h3 class="sub-title">Lisensi & Sertifikasi</h3>
        <ul class="certifications-list">
          <li v-for="cert in certifications" :key="cert.title">
            <strong>{{ cert.title }}</strong> - {{ cert.issuer }}
          </li>
        </ul>
      </div>
    </div>
  </section>
</template>

<script setup>
const coreSkills = [
  "Kotlin", "Android SDK", "Jetpack Compose", "MVVM/MVI Architecture",
  "Coroutines", "Dagger/Hilt", "Retrofit & OkHttp", "Room Database",
  "CI/CD", "Git", "Unit & UI Testing", "Agile Methodologies"
];
const certifications = [
  { title: "Associate Android Developer", issuer: "Google" },
  { title: "Kotlin for Java Developers", issuer: "Coursera" },
  { title: "Advanced Android with Kotlin", issuer: "Udacity" },
];
</script>

<style scoped>
.content-section {
  margin-bottom: 6rem;
  scroll-margin-top: 6rem;
}
.skills-block:not(:last-child) {
  margin-bottom: 2rem;
}
.sub-title {
  font-size: 1.25rem;
  font-weight: 600;
  color: white;
  margin-bottom: 1rem;
}
.skills-container {
  display: flex;
  flex-wrap: wrap;
  gap: 0.75rem;
}
.skill-badge {
  background-color: rgba(0, 246, 255, 0.1);
  color: var(--accent-primary);
  font-size: 0.875rem;
  font-weight: 500;
  padding: 0.5rem 1rem;
  border-radius: 0.5rem;
  border: 1px solid rgba(0, 246, 255, 0.2);
  transition: all 0.2s ease;
}
.skill-badge:hover {
  background-color: rgba(0, 246, 255, 0.2);
  color: white;
}
.certifications-list {
  list-style: none;
  padding-left: 0;
  display: flex;
  flex-direction: column;
  gap: 0.75rem;
}
.certifications-list li {
  color: var(--text-secondary);
}
.certifications-list li strong {
  color: var(--text-primary);
  font-weight: 600;
}
</style>
