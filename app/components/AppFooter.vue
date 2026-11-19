
<template>
  <footer class="footer">
    <div class="footer-content">
      <small>© 2026 ClassNest. All rights reserved.</small>

      <div class="social-links">
        <a
          href="https://www.facebook.com/richelleann.calabroso"
          target="_blank"
          rel="noopener noreferrer"
        >
          Facebook ↗
        </a>

        <a
          href="https://www.instagram.com/chelleann_1317/"
          target="_blank"
          rel="noopener noreferrer"
        >
          Instagram ↗
        </a>
      </div>
    </div>
  </footer>
</template>

<style scoped>
.footer {
  background-color: #F3EEE5;
  border-top: 1px solid #E6D8C3;
  padding: 20px 40px;
}

.footer-content {
  max-width: 1100px;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 15px;
}

small {
  color: #8A7968;
  font-size: 12px;
}

.social-links {
  display: flex;
  align-items: center;
  gap: 22px;
}

.social-links a {
  color: #5D866C;
  font-size: 12px;
  font-weight: bold;
  text-decoration: none;
  transition: color 0.3s ease;
}

.social-links a:hover {
  color: #453F38;
  text-decoration: underline;
}

@media (max-width: 500px) {
  .footer-content {
    flex-direction: column;
    gap: 12px;
  }
}
</style>
