
<script setup>
defineProps({
  label: {
    type: String,
    required: true
  },
  color: {
    type: String,
    default: '#5D866C'
  },
  to: {
    type: String,
    default: '/'
  }
})
</script>

<template>
  <NuxtLink
    :to="to"
    class="app-button"
    :style="{ backgroundColor: color }"
  >
    {{ label }}
  </NuxtLink>
</template>

<style scoped>
.app-button {
  display: inline-block;
  color: #FFFFFF;
  padding: 12px 24px;
  border-radius: 25px;
  text-decoration: none;
  font-size: 14px;
  font-weight: bold;
  transition: opacity 0.3s;
}

.app-button:hover {
  opacity: 0.8;
}
</style>
