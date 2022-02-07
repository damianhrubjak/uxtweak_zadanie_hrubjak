<template>
  <footer class="app-footer">
    <div class="page-width q-mx-auto bg-pallette-gray-warmer footer-wrapper">
      <div class="row page-wrapper">
        <div class="row col-12 col-md-8 footer-grid">
          <div
            class="footer-item"
            v-for="linkGroup in links"
            v-bind:key="linkGroup.name"
          >
            <p class="font-gray-text-darker font-black font-size-20px q-ml-sm">
              {{ linkGroup.name }}
            </p>
            <div v-for="item in linkGroup.items" v-bind:key="item">
              <FooterLink v-bind:label="item" />
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="page-width q-mx-auto q-pa-md text-center bg-pallette-white">
      <p class="q-ma-none">
        Copyright © 2021 UXtweak Research Group. All rights reserved.
      </p>
    </div>
  </footer>
</template>

<script>
import { defineComponent } from "vue";
import FooterLink from "../footer/footer-link.vue";

export default defineComponent({
  name: "Footer",

  components: { FooterLink },

  setup() {
    const links = [
      {
        name: "Product",
        items: ["Features", "Pricing", "Demos", "Consulting"],
      },
      {
        name: "Resources",
        items: ["Documentation", "Performance"],
      },
      {
        name: "Legal",
        items: [
          "Privacy by design",
          "GDPR compliance",
          "Terms of service",
          "Privacy policy",
          "Opt-out",
          "DPA",
        ],
      },
      {
        name: "Company",
        items: ["Contact", "Blog", "Careers"],
      },
    ];

    return {
      links,
    };
  },
});
</script>
