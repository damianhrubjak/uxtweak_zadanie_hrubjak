<template>
  <div
    class="nav-button-popup absolute-bottom bg-pallette-white shadow-2 rounded-borders q-pa-lg"
  >
    <slot />
  </div>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "MenuItemPopup",

  components: {},

  setup() {},
});
</script>
