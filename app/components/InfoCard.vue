<script setup>
defineProps({
  title: {
    type: String,
    required: true
  },
  description: {
    type: String,
    required: true
  }
})
</script>

<template>
  <div class="info-card">
    <h2>{{ title }}</h2>
    <p>{{ description }}</p>
  </div>
</template>

<style scoped>
.info-card {
  background-color: #E6D8C3;
  padding: 25px;
  border-radius: 12px;
  text-align: center;
}

h2 {
  color: #5D866C;
  font-size: 22px;
  margin-bottom: 12px;
}

p {
  color: #453F38;
  font-size: 15px;
  line-height: 1.6;
}
</style>
