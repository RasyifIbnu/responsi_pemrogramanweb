<template>
  <section class="hero-section">
    <div class="hero-content">
      <h1 class="text"><span class="highlight">Holla Amigos</span> Rasyif Ibnu</h1>
      <p>
       Hallo saya Ibnu AKA Kenoch ch saya adalah programer newbie <br>
      Salam Kenal  
      </p>
      <a class="btn btn-primary" href="http://www.youtube.com/@Nuninuch" role="button">Kenali Aku</a>
     
    </div>
    <div class="hero-image">
      <img src="../assets/img/pp.png" alt="Design Inspiration">
    </div>
  </section>
</template>

<script>
export default {
  name: 'HeroSection',
}
</script>

<style scoped>
.hero-section {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 4rem 2rem;
  background-color: #15bd26;
  color: #fff;
}

.hero-content {
  max-width: 50%;
}

.hero-content h1 {
  font-size: 3rem;
  line-height: 1.2;
}

.highlight {
  color: #8e44ad;
}

.hero-content p {
  font-size: 1rem;
  color: #ddd;
  margin: 1.5rem 0;
}
.text {
  color:aquamarine
}
.cta-button {
  padding: 1rem 2rem;
  border: 2px solid #8e44ad;
  background-color: transparent;
  color: #fff;
  font-size: 1rem;
  cursor: pointer;
  margin: 1rem 0;
  transition: background-color 0.3s, color 0.3s;
}

.cta-button:hover {
  background-color: #8e44ad;
  color: #fff;
}

.update-info {
  display: flex;
  align-items: center;
  font-size: 0.9rem;
  color: #ccc;
  margin-top: 1rem;
}

.update-icon {
  margin-right: 0.5rem;
}

.hero-image img {
  width: 400px;
  border-radius: 20%;
  margin-right: 300px;
}
</style>
