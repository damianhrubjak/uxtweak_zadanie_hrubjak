<template>
  <q-layout view="hHh lpR fFf" class="bg-pallette-gray">
    <!-- HEADER -->
    <Header />

    <q-page-container>
      <router-view />
    </q-page-container>

    <!-- HEADER -->
    <Footer />
  </q-layout>
</template>

<script>
import { defineComponent, ref } from "vue";
import Header from "src/components/header/header.vue";
import Footer from "src/components/footer/footer.vue";

export default defineComponent({
  name: "MainLayout",

  components: {
    Header,
    Footer,
  },

  setup() {
    return {};
  },
});
</script>
