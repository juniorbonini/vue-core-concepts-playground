<script setup>
import HelloWorld from "./components/HelloWorld/HelloWorld.vue";
</script>

<template>
  <header>
    <img
      class="logoImage"
      src="./images/logo.svg"
      alt="logo vite"
      width="125"
      height="125"
    />
    <div class="container">
      <HelloWorld message="Você conseguiu!" />
    </div>
  </header>

</template>

<style scoped>
header {
  line-height: 1.5;
}

.logoImage {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 64rem) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  .container {
    display: flex;
    place-content: flex-start;
    flex-wrap: wrap;
  }
}
</style>
