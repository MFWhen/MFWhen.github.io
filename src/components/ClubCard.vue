<template>
  <div class="club-card">
    <div class="club-logo">
      <img :src="club.logo" :alt="club.name" />
    </div>
    <div class="club-info">
      <h3>{{ club.name }}</h3>
      <p>{{ club.description }}</p>
      <a href="#" class="read-more">Read More</a>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    club: Object,
  },
};
</script>

