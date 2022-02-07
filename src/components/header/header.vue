<template>
  <header class="app-header">
    <div class="page-width q-mx-auto">
      <nav class="bg-pallette-white q-py-md">
        <div class="flex justify-between items-center page-wrapper">
          <div class="hamburger" @click="toggleMenu">
            <q-icon name="menu" size="2.5rem" color="font-gray-text-darker" />
          </div>
          <div class="flex items-center links-wrapper">
            <MenuItems />
          </div>
          <div>
            <q-btn outline color="primary" class="q-mr-sm" size="1rem">
              <div class="ghost-btn-stacked">
                <span class="text-dark text-bold block text-transform-none"
                  >Register</span
                >
                <span class="text-transform-none text-bold text-sm"
                  >for free</span
                >
              </div>
            </q-btn>
            <q-btn
              color="primary"
              size="1rem"
              unelevated
              class="text-transform-none"
            >
              Log In
            </q-btn>
          </div>
        </div>
      </nav>
    </div>
    <div
      :class="
        'side-menu fixed-top-right bg-pallette-white ' +
        (isToggled ? 'show' : '')
      "
    >
      <header class="flex justify-end q-pa-sm">
        <q-icon
          name="close"
          size="2rem"
          class="font-gray-text-darker"
          @click="toggleMenu"
        />
      </header>
      <div class="side-menu-items w-full q-mt-md">
        <MenuItems />
      </div>
    </div>
  </header>
</template>

<script>
import { defineComponent, ref } from "vue";

import MenuItems from "./menu-items";

export default defineComponent({
  name: "Header",

  components: {
    MenuItems,
  },

  setup() {
    const isToggled = ref(false);

    const toggleMenu = () => {
      isToggled.value = !isToggled.value;
    };
    return {
      isToggled,
      toggleMenu,
    };
  },
});
</script>
