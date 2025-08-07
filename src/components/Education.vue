<template>
  <section id="education" class="content-section">
    <h2 class="section-title">Pendidikan</h2>
    <div class="card">
      <div class="education-entry">
        <div>
          <h3 class="institution-name">Universitas Gadjah Mada (UGM)</h3>
          <p class="degree-name">Sarjana Teknik, Teknik Kimia</p>
        </div>
        <p class="education-years">2015 - 2020</p>
      </div>
    </div>
  </section>
</template>

<style scoped>
.content-section {
  margin-bottom: 6rem;
  scroll-margin-top: 6rem;
}
.education-entry {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  flex-wrap: wrap;
}
.institution-name {
  font-size: 1.25rem;
  font-weight: 600;
  color: white;
}
.degree-name {
  font-size: 1.125rem;
  font-weight: 500;
  color: var(--text-secondary);
}
.education-years {
  color: var(--accent-secondary);
  margin-top: 0.25rem;
  font-weight: 500;
}
</style>