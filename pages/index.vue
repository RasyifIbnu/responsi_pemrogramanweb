<template>
  <div>
    <HeroSection />
    <NavbarSection />
    <AboutSection/>
    <ContactSection/>
    <ProjectsSection/>
 
  </div>
</template>

<script>
import HeroSection from '~/components/HeroSection.vue';

import AboutSection from '~/components/AboutSection.vue';
import ProjectsSection from '~/components/ProjectsSection.vue';
import ContactSection from '~/components/ContactSection.vue';
import NavbarSection from '../components/NavbarSection.vue';





export default {
  components: {
    NavbarSection,
    HeroSection,
    AboutSection,
    ContactSection,
    ProjectsSection
  }
}
</script>./Index.vue
