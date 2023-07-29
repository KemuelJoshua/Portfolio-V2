<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-light fixed-top" :class="{
      'bg-transparent on-top': isTransparent,
      'bg-light': !isTransparent,
      'shadow-sm': !isTransparent
    }">
    <div class="container">
      <!-- Logo -->
      <a class="navbar-brand">
        <img src="../assets/img/logo-icon.png" alt="Logo" height="40">
      </a>

      <!-- Offcanvas Toggler Button for Mobile -->
      <button class="navbar-toggler" type="button" data-bs-toggle="offcanvas" data-bs-target="#navbarNav"
        aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>

      <!-- Offcanvas Navbar Items -->
      <div class="offcanvas offcanvas-end"  tabindex="-1" id="navbarNav">
        <div class="offcanvas-header bg-secondary">
          <h5 class="offcanvas-title text-dark">Menu</h5>
          <button type="button" class="btn-close text-reset" data-bs-dismiss="offcanvas" aria-label="Close"></button>
        </div>
        <div class="offcanvas-body color-bg">
          <ul class="navbar-nav ms-auto">
            <li class="nav-item" v-for="tab in tabs" :key="tab.id">
              <a class="nav-link" 
                :class="{
                  'text-white': isTransparent,
                  'dark': !isTransparent,
                  'active': (current === tab.route && tab.route === '#' + activeSection ) || tab.route === '#' + activeSection
                }"
                @click="isActiveLink(tab.route)"
                :href="tab.route">{{tab.name}}</a>
            </li>
            <li class="nav-item">
                <button @click="downloadResume" class="btn" :class="isTransparent ? 'btn-outline-third' : 'btn-outline-dark'">
                  Download Resume
                </button>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </nav>
</template>


<script>
export default {
  props: {
    // Define the 'active-section' prop
    activeSection: {
      type: String,
      default: null
    }
  },
    data(){
        return {
            isTransparent: true,
            current: null,
            resumePath: '../assets/resume.pdf',
            tabs: [
              {id: 1, name: 'Home', route: '#home'},
              {id: 2, name: 'about', route: '#about'},
              {id: 3, name: 'Portfolio', route: '#portfolio'},
              {id: 4, name: 'leadership', route: '#leadership'},
            ]
        }
    },
    mounted() {
    window.addEventListener('scroll', this.handleScroll);
    },
    beforeDestroy() {
        window.removeEventListener('scroll', this.handleScroll);
    },
    methods: {
        handleScroll() {
        this.isTransparent = window.scrollY === 0;
        },
        isActiveLink(link) {
          this.current = link;
        },
        downloadResume() {
          window.open(this.resumePath, '_blank');
        }
    },
}
</script>

<style lang="scss" scoped>

  
.on-top {
    height: 110px;
    transition: all .8s ease;
}

.bg-light {
    transition: all .8s ease;
    padding: 20px;
}

.nav-item {
    padding-left: 10px;
    padding-right: 10px;
    text-transform: uppercase;
}


@media (max-width: 991px) {
  .color-bg {
    background-color: #5be9b9;
  }
}
</style>