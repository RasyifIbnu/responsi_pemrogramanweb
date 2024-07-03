<template>
  <section id="projects" class="project-section py-5">
    <div class="container">
      <h2 class="text-center mb-4">My Projects</h2>
      <div class="row justify-content-center">
        <div class="col-lg-4 col-md-6 mb-4" v-for="project in projects" :key="project.id">
          <div class="card shadow-sm border-0">
            <img :src="project.image" class="card-img-top rounded" alt="Project Image">
            <div class="card-body">
              <h5 class="card-title">{{ project.title }}</h5>
              <p class="card-text">{{ project.description }}</p>
              <a :href="project.link" class="btn btn-primary stretched-link" target="_blank">View Project</a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import Jam from '@/assets/img/jam.jpg'
import Ai from '@/assets/img/ai.jpg'

export default {
  name: 'ProjectSection',

  data() {
    return {
      projects: [
        {
          id: 1,
          title: 'Simple Digital Watch',
          description: 'Saya membuat ini untuk belajar tutorial dari Tiktok',
          image: Jam,
          link: 'https://github.com/RasyifIbnu/jam_digital.git'
        },
        {
          id: 2,
          title: 'Artificial Intelligence ',
          description: 'Saya membuat ini untuk tugas mata kuliah Kecerdasan Buatan',
          image: Ai,
          link: 'https://colab.research.google.com/drive/15lKWc96r2g1ZruoukbA8Wde_THRa5-Dw?usp=sharing'
        },
        // Add more projects here
      ]
    }
  }
}
</script>

<style scoped>
.project-section {
  background: linear-gradient(to right, #a6c0fe, #84fab0);
  padding: 80px 0;
}

.card {
  transition: transform 0.3s;
}

.card:hover {
  transform: translateY(-5px);
}

.card img {
  transition: transform 0.3s;
}

.card:hover img {
  transform: scale(1.1);
}

.card-title {
  font-size: 1.25rem;
  color: #333;
}

.card-text {
  color: #666;
}

.btn-primary {
  background-color: #8e44ad;
  border-color: #8e44ad;
}

.btn-primary:hover {
  background-color: #722b8b;
  border-color: #722b8b;
}
</style>
