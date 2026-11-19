
<script setup>
defineProps({
  name: {
    type: String,
    required: true
  },
  course: {
    type: String,
    required: true
  },
  image: {
    type: String,
    required: true
  },
  description: {
    type: String,
    required: true
  },
  github: {
    type: String,
    default: ''
  }
})
</script>

<template>
  <article class="student-card">

    <!-- Profile Picture -->
    <div class="image-container">
      <img :src="image" :alt="name" class="profile-image">
    </div>

    <!-- Student Information -->
    <div class="student-info">
      <span class="student-label">ITE 18 STUDENT</span>

      <h2>{{ name }}</h2>

      <p class="course">{{ course }}</p>

      <div class="card-divider"></div>

      <p class="description">{{ description }}</p>

      <!-- GitHub Profile -->
      <a
        v-if="github"
        :href="github"
        target="_blank"
        rel="noopener noreferrer"
        class="github-link"
      >
        GitHub Profile ↗
      </a>
    </div>

  </article>
</template>

<style scoped>
.student-card {
  background-color: #FFFFFF;
  border: 1px solid #E6D8C3;
  border-radius: 16px;
  overflow: hidden;
  box-shadow: 0 5px 18px rgba(69, 63, 56, 0.06);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.student-card:hover {
  transform: translateY(-6px);
  box-shadow: 0 12px 25px rgba(69, 63, 56, 0.12);
}

.image-container {
  width: 100%;
  height: 260px;
  overflow: hidden;
  background-color: #E6D8C3;
}

.profile-image {
  width: 100%;
  height: 100%;
  object-fit: cover;
  object-position: center;
  display: block;
  transition: transform 0.4s ease;
}

.student-card:hover .profile-image {
  transform: scale(1.04);
}

.student-info {
  padding: 24px;
  text-align: left;
}

.student-label {
  color: #5D866C;
  font-size: 11px;
  font-weight: bold;
  letter-spacing: 1.5px;
}

h2 {
  color: #453F38;
  font-size: 20px;
  margin: 10px 0 6px;
}

.course {
  color: #8A7968;
  font-size: 13px;
}

.card-divider {
  height: 1px;
  background-color: #E6D8C3;
  margin: 16px 0;
}

.description {
  color: #665F56;
  font-size: 14px;
  line-height: 1.7;
}

.github-link {
  display: inline-block;
  margin-top: 16px;
  color: #5D866C;
  font-size: 13px;
  font-weight: bold;
  text-decoration: none;
}

.github-link:hover {
  color: #453F38;
  text-decoration: underline;
}
</style>
