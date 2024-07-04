<template>
  <div>
    <HeroSection />
    <NavbarSection />
    <AboutSection/>
    <ContactSection/>
    <ProjectsSection/>
    <FooterSection/> 
 
  </div>
</template>

<script>

import HeroSection from '~/components/HeroSection.vue';

import AboutSection from '~/components/AboutSection.vue';
import ProjectsSection from '~/components/ProjectsSection.vue';
import ContactSection from '~/components/ContactSection.vue';
import NavbarSection from '../components/NavbarSection.vue';
import FooterSection from '../components/FooterSection.vue';




export default {
  components: {
    
    NavbarSection,
    HeroSection,
    AboutSection,
    ContactSection,
    ProjectsSection,
    FooterSection,
  }
}
</script>./Index.vue
