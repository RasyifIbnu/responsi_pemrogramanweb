<template>
  <section class="project-section py-5">
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
export default {
  name: 'ProjectSection',
  data() {
    return {
      projects: [
        {
          id: 1,
          title: 'Project One',
          description: 'This is a description for project one. Lorem ipsum dolor sit amet, consectetur adipiscing elit.',
          image: 'https://via.placeholder.com/300x200',
          link: '#'
        },
        {
          id: 2,
          title: 'Project Two',
          description: 'This is a description for project two. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas.',
          image: 'https://via.placeholder.com/300x200',
          link: '#'
        },
        // Add more projects here
      ]
    }
  }
}
</script>

<style scoped>
.project-section {
  background-color: #f9f9f9;
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
