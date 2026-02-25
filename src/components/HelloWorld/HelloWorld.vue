<script setup>
defineProps({
  message: {
    type: String,
    required: true,
  },
});
</script>

<template>
  <div class="container">
    <h1 class="title">{{ message }}</h1>
    <h3>
      Você criou com sucesso um projeto com
      <a href="https://vite.dev/">Vite</a> +
      <a href="https://vuejs.org/">Vue3</a>
    </h3>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  position: realtive;
  top: -0.625rem;
}

h3 {
  font-size: 1.2rem;
}

.container h1,
.container h3 {
  text-align: center;
}

@media (min-width: 64rem) {
  .container h1,
  .container h3 {
    text-align: left;
  }
}
</style>
