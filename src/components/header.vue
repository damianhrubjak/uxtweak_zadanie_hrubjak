<template>
  <header class="app-header">
    <div class="page-width q-mx-auto">
      <nav
        class="flex justify-between items-center bg-pallette-white q-px-8-75 q-py-md"
      >
        <div class="flex items-center">
          <button
            class="nav-button cursor-pointer text-bold q-px-md q-py-sm flex items-center rounded-borders"
            name="features-tab"
          >
            <span>Features</span>
            <q-icon
              class="yellow-icon q-ml-sm"
              name="arrow_drop_down"
              size="26px"
            />
          </button>
          <button
            class="nav-button cursor-pointer text-bold q-px-md q-py-sm flex items-center rounded-borders"
            name="pricing-tab"
          >
            <span>Pricing</span>
          </button>
          <button
            class="nav-button cursor-pointer text-bold q-px-md q-py-sm flex items-center rounded-borders"
            name="contact-tab"
          >
            <span>Contact</span>
            <q-icon
              class="yellow-icon q-ml-sm"
              name="arrow_drop_down"
              size="26px"
            />
          </button>
          <button
            class="nav-button cursor-pointer text-bold q-px-md q-py-sm flex items-center rounded-borders"
            name="learn-tab"
          >
            <span>Learn</span>
            <q-icon
              class="yellow-icon q-ml-sm"
              name="arrow_drop_down"
              size="26px"
            />
          </button>
        </div>
        <div>
          <q-btn outline color="primary" class="q-mr-sm" size="1rem">
            <div class="ghost-btn-stacked">
              <span class="text-dark text-bold block text-transform-none"
                >Register</span
              >
              <span class="text-transform-none text-bold">for free</span>
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
      </nav>
    </div>
  </header>
</template>

<script>
import { defineComponent, reactive } from "vue";

export default defineComponent({
  name: "Header",

  components: {},

  setup() {},
});
</script>
