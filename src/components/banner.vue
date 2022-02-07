<template>
  <div class="w-full q-py-xl">
    <h2 class="font-black font-gray-text-darker q-my-md">{{ heading }}</h2>
    <h5 class="font--yellow font-black q-my-none">
      {{ subHeading }}
    </h5>
  </div>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "Banner",

  props: {
    heading: String,
    subHeading: String,
  },
});
</script>

<style></style>
