<template>
  <section id="hero" class="hero-section">
    <div class="profile-picture-container">
      <img 
        src="https://media.licdn.com/dms/image/v2/D5603AQHDaTcZYIXc6A/profile-displayphoto-shrink_800_800/B56ZebhH1kHUAg-/0/1750660841600?e=1757548800&v=beta&t=I7uNBCOkqU9dvcChNIcTg9sYmRLO19bdb1q3fu_NoK8"
        alt="Foto Profil Hadyan Jazila Subagja"
        class="profile-picture"
      />
    </div>
    <h1 class="hero-title">Hadyan Jazila Subagja</h1>
    <p class="hero-subtitle">Android Developer | <span class="gradient-text">Kotlin & Jetpack Compose</span> Specialist</p>
    <p class="hero-description">Membangun aplikasi seluler yang skalabel dan berpusat pada pengguna, mengubah ide menjadi pengalaman Android yang menarik.</p>
    <a href="#contact" class="hero-cta-button">
      Hubungi Saya <i class="fas fa-arrow-right"></i>
    </a>
  </section>
</template>

<style scoped>
.hero-section {
  text-align: center;
  margin-bottom: 8rem;
  padding-top: 4rem;
}
.profile-picture-container {
  position: relative;
  width: 10rem;
  height: 10rem;
  margin: 0 auto 2rem auto;
}
.profile-picture-container::before {
  content: '';
  position: absolute;
  inset: -5px;
  border-radius: 50%;
  background: conic-gradient(from 90deg at 50% 50%, var(--accent-primary), var(--accent-secondary), var(--accent-primary));
  animation: spin 3s linear infinite;
  z-index: -1;
}
@keyframes spin {
  from { transform: rotate(0deg); }
  to { transform: rotate(360deg); }
}
.profile-picture {
  width: 100%;
  height: 100%;
  object-fit: cover;
  border-radius: 50%;
  border: 4px solid var(--bg-dark);
}
.hero-title {
  font-size: 3.5rem;
  font-weight: 800;
  color: white;
  margin-bottom: 0.5rem;
}
.hero-subtitle {
  font-size: 1.25rem;
  color: var(--text-primary);
  margin-bottom: 1.5rem;
}
.gradient-text {
  background: linear-gradient(90deg, var(--accent-primary), var(--accent-secondary));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  font-weight: 600;
}
.hero-description {
  max-width: 42rem;
  margin: 0 auto 2.5rem auto;
  color: var(--text-secondary);
  line-height: 1.6;
}
.hero-cta-button {
  background: linear-gradient(90deg, var(--accent-primary), var(--accent-secondary));
  color: #0a0f1f;
  font-weight: 700;
  padding: 1rem 2.5rem;
  border-radius: 0.5rem;
  text-decoration: none;
  transition: all 0.3s ease;
  box-shadow: 0 0 20px rgba(0, 246, 255, 0.3);
}
.hero-cta-button:hover {
  transform: translateY(-3px);
  box-shadow: 0 0 30px rgba(0, 246, 255, 0.5);
}
.hero-cta-button i {
  margin-left: 0.5rem;
  transition: transform 0.2s ease-in-out;
}
.hero-cta-button:hover i {
  transform: translateX(5px);
}
</style>