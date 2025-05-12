<template>
  <section class="hero">
    <img src="@/assets/smu.png" alt="Campus Building" />
    <div class="hero-content">
      <h1>SMU Connect</h1>
      <button class="join-btn">Join a Club</button>
    </div>
  </section>
</template>

<style scoped>
.hero {
  position: relative;
  height: 400px;
  width: 100%;
  overflow: hidden;
}

.hero img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.hero-content {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: flex-start;
  padding: 0 50px;
  background: linear-gradient(to right, rgba(0, 0, 0, 0.6), rgba(0, 0, 0, 0.3));
}

.hero-content h1 {
  color: white;
  font-size: 40px;
  margin-bottom: 25px;
}

.join-btn {
  background-color: white;
  color: #0078a8;
  border: none;
  padding: 12px 24px;
  border-radius: 4px;
  font-size: 16px;
  cursor: pointer;
  font-weight: bold;
  transition: all 0.3s;
}

.join-btn:hover {
  background-color: #f0f0f0;
  transform: translateY(-2px);
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}
</style>