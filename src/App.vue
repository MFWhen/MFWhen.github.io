<script>
import ClubCard from './components/ClubCard.vue';
import ClubsSection from './components/ClubsSection.vue';
import Footer from './components/Footer.vue';
import Header from './components/Header.vue';
import HeroSection from './components/HeroSection.vue';



export default {
  components: {
    Header,
    Footer,
    HeroSection,
    ClubsSection,
    ClubCard
  },
};
</script>

<template>
  <div id="app">
    <Header />
    <HeroSection />
    <AboutSection />
    <ClubsSection />
    <Footer />
  </div>
</template>

<style scoped>
#app {
  background-color: white; 
  color: #333; 
  min-height: 100vh; 
  margin: 0; 
  padding: 0;
  display: flex;
  flex-direction: column;
}

header,
section,
footer {
  width: 100%; 
  margin: 0; 
  padding: 0; 
  flex-shrink: 0;
}
</style>

