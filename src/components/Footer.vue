<template>
  <footer class="footer">
    <p>&copy; {{ currentYear }} Hadyan Jazila Subagja. </p>
  </footer>
</template>

<script setup>
const currentYear = new Date().getFullYear();
</script>

<style scoped>
.footer {
  background-color: transparent;
  color: var(--text-secondary);
  margin-top: 5rem;
  padding: 2rem 1.5rem;
  text-align: center;
  border-top: 1px solid var(--border-color);
}
.icon-heart {
  color: var(--accent-primary);
}
</style>