<template>
  <section class="clubs-section">
    <h2>OUR CLUBS</h2>
    <div class="clubs-container">
      <div v-for="club in clubs" :key="club.id" class="club-card">
        <div class="club-logo">
          <img :src="club.logo" :alt="club.name" />
        </div>
        <div class="club-info">
          <h3>{{ club.name }}</h3>
          <p>{{ club.description }}</p>
           <a :href="club.link" class="read-more" target="_blank" rel="noopener noreferrer">Read More</a>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      clubs: [
        {
          id: 1,
          name: "IEEE",
          logo: "src\\assets\\ieee.png",
          description: "The Institute of Electrical and Electronics Engineers (IEEE)...",
          link: "https://www.ieee.org/",
        },
        {
          id: 2,
          name: "Google Developer Club",
          logo: "src\\assets\\gdg.png",
          description: "Join a Google community for developers to network, share stories, and learn together about web and mobile app development, cloud, AI, and other topics...",
          link: "https://developers.google.com/community/gdg",
        },
        {
          id: 3,
          name: "Lions Club",
          logo: "src\\assets\\Lions_Clubs_International_logo.svg.png",
          description: "Lions Club is a place where individuals join together to improve their communities...",
          link: "https://www.lionsclubs.org/en",
        },
      ],
    };
  },
};
</script>

<style scoped>
.clubs-section {
  padding: 60px 40px;
  background-color: #f8f8f8;
  text-align: center;
}

.clubs-container {
  display: flex;
  justify-content: space-between;
  gap: 30px;
  flex-wrap: wrap;
}

.club-card {
  background-color: white;
  border-radius: 8px;
  overflow: hidden;
  box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
  flex: 1;
  max-width: 300px;
  transition: transform 0.3s;
}

.club-card:hover {
  transform: translateY(-10px);
}

.club-logo img {
  width: 100%;
  height: 150px;
  object-fit: cover;
}

.club-info {
  padding: 20px;
  text-align: left;
}

.club-info h3 {
  margin-bottom: 10px;
  color: #333;
  font-size: 20px;
}

.club-info p {
  color: #666;
  font-size: 14px;
  line-height: 1.5;
  margin-bottom: 15px;
  height: 80px;
  overflow: hidden;
}

.read-more {
  color: #0078a8;
  text-decoration: none;
  font-size: 14px;
  font-weight: bold;
}

.read-more:hover {
  text-decoration: underline;
}
</style>