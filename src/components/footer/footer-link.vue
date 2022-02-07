<template>
  <q-btn
    :label="label"
    flat
    class="w-full text-left font--gray-text-warmer footer-link"
    align="left"
    padding="10px"
    size="1rem"
    no-caps
  ></q-btn>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "FooterLink",

  props: {
    label: String,
  },

  setup() {
    return {};
  },
});
</script>
