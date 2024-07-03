<template>
  <section id="home" class="hero-section">
    <div class="hero-content">
      <h1 class="text"><span class="highlight">Holla Amigos</span> I am Rasyif Ibnu</h1>
      <p>
       Hallo saya Ibnu AKA Kenoch ch saya adalah mahasiswa disalah satu universitas swasta terkenal di Indonesia <br>
      Saya membuat website ini untuk sarana mengimplementasikan hasil belajar saya dalam mata kuliah Pemrograman Web.    
      </p>
      <a class="btn btn-primary" href="http://www.youtube.com/@Nuninuch" role="button">Channel youtube </a>
     
    </div>
    <div data-aos="fade-up-left" class="hero-image">
      <img src="../assets/img/ppcopy.png" alt="Design Inspiration">
    </div>
  </section>
</template>

<script>
export default {
  name: 'HeroSection',
  mounted() {
    // Memastikan AOS diinisialisasi setelah komponen dimuat
    this.$nextTick(() => {
      this.$AOS.refresh()
  })
}
}
</script>

<style scoped>
body {
  background: linear-gradient(to right, #a6c0fe, #84fab0); /* Set the body background to match the sections */
  margin: 0;
  border: none;
}

.hero-section {
  background: linear-gradient(to right, #a6c0fe, #84fab0);
  color: #fff;
  padding: 10rem;
  display: flex;
  align-items: center;
  justify-content: space-between;
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
  color: aquamarine;
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
}
</style>
