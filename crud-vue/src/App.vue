<script setup>
import HomeViewVue from "./views/HomeView.vue";
import StudentView from '../src/views/Students/View.vue'
</script>

<template>
  <header>
    <div class="wrapper">
      <nav class="navbar navbar-expand-lg bg-body-tertiary bg-dark">
        <div class="container-fluid">
          <RouterLink class="navbar-brand" to="/">Home</RouterLink>
          <button
            class="navbar-toggler"
            type="button"
            data-bs-toggle="collapse"
            data-bs-target="#navbarSupportedContent"
            aria-controls="navbarSupportedContent"
            aria-expanded="false"
            aria-label="Toggle navigation"
          >
            <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav me-auto mb-2 mb-lg-0">
              <li class="nav-item">
                <RouterLink class="nav-link active" to="/">Home</RouterLink>
              </li>
              <li class="nav-item">
                <RouterLink class="nav-link active" to="/students"
                  >Students</RouterLink
                >
              </li>
            </ul>
          </div>
        </div>
      </nav>
    </div>
    <RouterView />
  </header>
</template>

<style scoped>
</style>
