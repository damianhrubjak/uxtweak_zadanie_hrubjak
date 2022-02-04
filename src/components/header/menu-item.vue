<template>
  <div
    role="button"
    class="nav-button font-size-16px cursor-pointer q-px-md q-py-sm flex items-center rounded-borders"
  >
    <span class="text-bold">{{ label }}</span>
    <q-icon
      class="yellow-icon q-ml-sm"
      name="arrow_drop_down"
      size="26px"
      v-if="isDropDown"
    />

    <slot v-if="isDropDown" />
  </div>
</template>

<script>
import { defineComponent, reactive } from "vue";

export default defineComponent({
  name: "MenuItem",

  props: {
    label: String,
    isDropDown: Boolean,
  },

  components: {},

  setup() {},
});
</script>
