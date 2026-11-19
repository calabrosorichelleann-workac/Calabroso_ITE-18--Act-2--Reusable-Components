<template>
  <header class="header">
    <div class="container">
      <NuxtLink to="/" class="logo">
        ClassNest
      </NuxtLink>

      <nav class="navigation">
        <NuxtLink to="/">Home</NuxtLink>
        <NuxtLink to="/students">Students</NuxtLink>
      </nav>
    </div>
  </header>
</template>

<style scoped>
.header {
  background-color: #5D866C;
  padding: 20px 40px;
}

.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 1100px;
  margin: 0 auto;
}

.logo {
  color: #F5F5F0;
  font-size: 24px;
  font-weight: bold;
  text-decoration: none;
}

.navigation {
  display: flex;
  gap: 25px;
}

.navigation a {
  color: #F5F5F0;
  text-decoration: none;
  font-size: 16px;
}

.navigation a:hover {
  color: #E6D8C3;
}
</style>
