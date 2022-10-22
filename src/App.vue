<script setup>
import projects from "@/components/projects.vue";
import contact from "@/components/contact.vue";
</script>

<template>
  <div class="layout text-white">
    <header>
      <!-- Fixed navbar -->
      <nav class="navbar navbar-expand-md navbar-dark fixed-top">
        <div class="container">
          <a class="navbar-brand" href="#">张渊明</a>
          <button
            class="navbar-toggler"
            type="button"
            data-bs-toggle="collapse"
            data-bs-target="#navbarCollapse"
            aria-controls="navbarCollapse"
            aria-expanded="false"
            aria-label="Toggle navigation"
          >
            <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse" id="navbarCollapse">
            <ul class="navbar-nav me-auto mb-2 mb-md-0">
              <li class="nav-item">
                <a class="nav-link" href="#projects">Projects</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#contact">Contact</a>
              </li>
            </ul>
          </div>
        </div>
      </nav>
    </header>

    <!-- Intro Section -->
    <section id="banner" class="slide-portfolio">
      <div class="pixel"></div>
      <div class="container">
        <div class="row">
          <div class="col-sm-12 profile">
            <figure class="image">
              <img
                class="img-fluid rounded-circle"
                src="@/assets/img/foto.png"
              />
            </figure>
            <h1 class="text-center">Yohn Cheung</h1>
            <p class="lead text-center">
              A professional working as a Vue developer. Currently rebuilding
              software applications and adding new features for social work and
              welfare domains.
            </p>

            <p class="text-center">
              Vue.js | HMTL5 | CSS3 | Javscript | Bootstrap | Quasar
            </p>
            <!--<a class="page-scroll glyphicon glyphicon-chevron-down arrow" href="#about"></a>-->
          </div>
        </div>
      </div>
    </section>

    <section class="container px-4 py-5" id="projects">
      <projects />
    </section>

    <section class="container px-4 py-5" id="contact">
      <contact />
    </section>
  </div>
</template>

<style scoped>
.layout,
.navbar {
  background-color: #363636;
}

#banner {
  margin-top: 50px;
  min-height: 100%;
  height: 100%;
  width: 100%;
  max-width: 100%;
  position: relative;
  background: url(@/assets/img/2.png) 50% 0 repeat fixed;
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  background-size: cover;
  box-shadow: inset 0 0 0 300px rgba(0, 0, 0, 0.3);
}

.pixel {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: url(@/assets/img/pixel.png);
  background-color: rgba(0, 0, 0, 0.4);
}

.slide-portfolio {
  /*height: 100%;*/
  padding-top: 50px;
  background: #ffffff;
  padding: 50px 0 30px 0;
}

.profile {
  z-index: 10;
}

.image {
  display: block;
  margin-left: auto;
  margin-right: auto;
  width: 20%;
  z-index: 10;
}
</style>
