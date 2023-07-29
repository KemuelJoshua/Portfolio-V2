<template>
  <div>
    <navbar-component :active-section="activeSection" />
    <div id="home">
      <homePageVue />
    </div>
    <div class="bg-white" id="about">
      <aboutMe/>
    </div>
    <div class="bg-white2" id="portfolio">
      <portfolio-component/>
    </div>
    <div class="bg-white" id="leadership">
      <leadershipVue/>
    </div>
    <footerComponentVue id="footer" />
  </div>
</template>

<script>
import aboutMe from '@/components/aboutMe.vue';
import NavbarComponent from '@/components/NavbarComponent.vue';
import leadershipVue from '@/components/LeadershipExpi.vue';
import footerComponentVue from '@/components/footerComponent.vue';
import homePageVue from '../pages/homePage.vue';
import PortfolioComponent from '../components/portfolioComponent.vue';

export default {
  name: 'contentView',
  components: {
    homePageVue,
    NavbarComponent,
    footerComponentVue,
    aboutMe,
    leadershipVue,
    PortfolioComponent
  },
  data() {
    return {
      activeSection: null
    };
  },
  mounted() {
    window.addEventListener('scroll', this.handleScroll);
    this.handleScroll(); // Call handleScroll initially to set the activeSection if needed
  },
  destroyed() {
    window.removeEventListener('scroll', this.handleScroll);
  },
  methods: {
    handleScroll() {
      const sections = ['home', 'about', 'portfolio', 'leadership', 'footer']; // Add more sections' IDs here if needed
      for (const section of sections) {
        const el = document.getElementById(section);
        if (el && this.isElementInViewport(el)) {
          this.activeSection = section;
          this.$emit('the-route', section); // Emit the event with the active section ID
          break;
        }
      }
    },
    isElementInViewport(el) {
      const rect = el.getBoundingClientRect();
      const windowHeight = window.innerHeight || document.documentElement.clientHeight;
      return rect.top < windowHeight && rect.bottom > 0;
    }
  }
};
</script>
