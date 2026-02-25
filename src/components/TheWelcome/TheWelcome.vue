<script setup>
import Container from "@/components/Item/item.vue";
import IconDoc from "@/components/icons/IconDocumentation.vue";
import IconSupport from "@/components/icons/IconSupport.vue";
import IconEco from "@/components/icons/IconEcoSystem.vue";
import IconTool from "@/components/icons/IconTooling.vue";
import IconCommunity from "../icons/IconCommunity.vue";

const openReadmeEditor = () => fetch("/__open-in-editor?file=README.md");
</script>

<template>
  <Container>
    <template #icon>
      <IconDoc />
    </template>
    <template #heading>Documentação</template>

    A
    <a href="https://vuejs.org/" target="_blank" rel="noopener">
      documentação oficial do Vue
    </a>
    fornece todas as informações necessárias para você começar.
  </Container>

  <Container>
    <template #icon>
      <IconTool />
    </template>
    <template #heading>Ferramentas</template>

    Este projeto é servido e empacotado com o
    <a
      href="https://vite.dev/guide/features.html"
      target="_blank"
      rel="noopener"
      >Vite</a
    >. A configuração de IDE recomendada é
    <a href="https://code.visualstudio.com/" target="_blank" rel="noopener">
      VSCode
    </a>
    +
    <a
      href="https://github.com/vuejs/language-tools"
      target="_blank"
      rel="noopener"
      >Vue - Official</a
    >. Se você precisar testar seus componentes e páginas web, confira:
    <a href="https://vitest.dev/" target="_blank" rel="noopener">Vitest</a>
    e
    <a href="https://www.cypress.io/" target="_blank" rel="noopener">Cypress</a>
    /
    <a href="https://playwright.dev/" target="_blank" rel="noopener">
      Playwright </a
    >.

    <br />

    Mais instruções estão disponíveis em
    <a href="javascript:void(0)" @click="openReadmeInEditor">
      <code>README.md</code> </a
    >.
  </Container>

  <Container>
    <template #icon>
      <IconEco />
    </template>
    <template #heading>Ecossistema</template>

    Obtenha ferramentas e bibliotecas oficiais para o seu projeto:
    <a href="https://pinia.vuejs.org/" target="_blank" rel="noopener">Pinia</a>,
    <a href="https://router.vuejs.org/" target="_blank" rel="noopener">
      Vue Router </a
    >,
    <a href="https://test-utils.vuejs.org/" target="_blank" rel="noopener">
      Vue Test Utils
    </a>
    e
    <a href="https://github.com/vuejs/devtools" target="_blank" rel="noopener">
      Vue Dev Tools </a
    >. Se precisar de mais recursos, recomendamos visitar o
    <a
      href="https://github.com/vuejs/awesome-vue"
      target="_blank"
      rel="noopener"
      >Awesome Vue</a
    >.
  </Container>

  <Container>
    <template #icon>
      <IconCommunity />
    </template>
    <template #heading>Comunidade</template>

    Ficou travado em algum ponto? Tire sua dúvida no
    <a href="https://chat.vuejs.org" target="_blank" rel="noopener">
      Vue Land
    </a>
    (servidor oficial no Discord) ou no
    <a
      href="https://stackoverflow.com/questions/tagged/vue.js"
      target="_blank"
      rel="noopener"
      >StackOverflow</a
    >. Você também pode seguir o perfil oficial
    <a href="https://bsky.app/profile/vuejs.org" target="_blank" rel="noopener">
      @vuejs.org
    </a>
    no Bluesky ou o
    <a href="https://x.com/vuejs" target="_blank" rel="noopener"> @vuejs </a>
    no X para acompanhar as novidades do mundo Vue.
  </Container>

  <Container>
    <template #icon>
      <IconSupport />
    </template>
    <template #heading>Apoie o Vue</template>

    Como um projeto independente, o Vue depende do apoio da comunidade para se
    manter. Você pode ajudar
    <a href="https://vuejs.org/sponsor/" target="_blank" rel="noopener">
      tornando-se um patrocinador </a
    >.
  </Container>
</template>
