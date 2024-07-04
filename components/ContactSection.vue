<template>
  <section  id="contact" class="contact-section">
    <div data-aos="flip-up" class="card">
      <h2>Contact Me</h2>
      <form @submit.prevent="submitForm">
        <div class="form-group">
          <label for="name">Name</label>
          <input type="text" id="name" v-model="form.name" required>
        </div>
        <div class="form-group">
          <label for="email">Email</label>
          <input type="email" id="email" v-model="form.email" required>
        </div>
        <div class="form-group">
          <label for="message">Message</label>
          <textarea id="message" v-model="form.message" required></textarea>
        </div>
        <button type="submit" class="submit-button" href="#home">Send Message</button>
      </form>
    </div>
  </section>
</template>

<script>
import HeroSection from '~/components/HeroSection.vue';

export default {
  name: 'ContactSection',
  mounted() {
    // Memastikan AOS diinisialisasi setelah komponen dimuat
    this.$nextTick(() => {
      this.$AOS.refresh()
  })
},

components: {
  HeroSection,
},
  data() {
    return {
      form: {
        name: '',
        email: '',
        message: ''
      }
    }
  },
  methods: {
    submitForm() {
      // Handle form submission logic here
      console.log('Form submitted', this.form)
      // Reset form
      this.form.name = ''
      this.form.email = ''
      this.form.message = ''
    }
  }
}
</script>

<style scoped>
.contact-section {
  background: linear-gradient(to right, #a6c0fe, #84fab0);
  color: #26bcc1;
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
  padding: 2rem;
  background-color: #f9f9f9;
  color: #333;
}

.card {
  background: #fff;
  padding: 2rem;
  border-radius: 8px;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
  max-width: 500px;
  width: 100%;
}

.contact-section h2 {
  text-align: center;
  margin-bottom: 2rem;
  font-size: 2rem;
  color: #8e44ad;
}

.form-group {
  margin-bottom: 1.5rem;
}

.form-group label {
  display: block;
  margin-bottom: 0.5rem;
  font-weight: bold;
}

.form-group input,
.form-group textarea {
  width: 100%;
  padding: 0.75rem;
  border: 1px solid #ddd;
  border-radius: 4px;
  font-size: 1rem;
}

.form-group textarea {
  resize: vertical;
  height: 150px;
}

.submit-button {
  display: block;
  width: 100%;
  padding: 1rem;
  background-color: #1649af;
  color: #fff;
  border: none;
  border-radius: 4px;
  font-size: 1.2rem;
  cursor: pointer;
  transition: background-color 0.3s;
}

.submit-button:hover {
  background-color: #722b8b;
}
</style>
