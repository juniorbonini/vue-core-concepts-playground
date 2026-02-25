<script setup>
import IconDoc from "@/components/icons/IconCommunity.vue";
import IconSupport from "@/components/icons/IconSupport.vue";
import IconEco from "@/components/icons/IconEcoSystem.vue";
import IconTool from "@/components/icons/IconTooling.vue";

const openReadmeEditor = () => fetch("/__open-in-editor?file=README.md");
</script>

<template>
  <h1>Welcome item aqui</h1>
  <template .icon>
    <IconDoc />
  </template>
</template>
