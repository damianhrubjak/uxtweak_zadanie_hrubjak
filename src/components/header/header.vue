<template>
  <header class="app-header">
    <div class="page-width q-mx-auto">
      <nav
        class="flex justify-between items-center bg-pallette-white q-px-8-75 q-py-md"
      >
        <div class="flex items-center">
          <MenuItem label="Features" isDropDown>
            <MenuItemPopup>
              <div class="row">
                <p class="q-mb-none font-black">Features</p>
              </div>
            </MenuItemPopup>
          </MenuItem>
          <MenuItem label="Pricing" />
          <MenuItem label="Contact" isDropDown>
            <MenuItemPopup>
              <div class="flex items-start row">
                <div class="item col">
                  <p class="q-mb-none font-black">Contact Form</p>
                  <p class="q-mb-none text-sm">Feel free to send us message</p>
                </div>
                <div class="item col q-ml-md">
                  <p class="q-mb-none font-black">Schedule live demo</p>
                  <p class="q-mb-none font-size-14px font-medium">
                    Book a live demo wit our product specialist
                  </p>
                </div>
              </div>
            </MenuItemPopup>
          </MenuItem>
          <MenuItem label="Learn" isDropDown>
            <MenuItemPopup>
              <div class="row">
                <p class="q-mb-none font-black">Learn with us</p>
              </div>
            </MenuItemPopup>
          </MenuItem>
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
      </nav>
    </div>
  </header>
</template>

<script>
import { defineComponent, reactive } from "vue";
import MenuItem from "./menu-item";
import MenuItemPopup from "./menu-item-popup";

export default defineComponent({
  name: "Header",

  components: {
    MenuItem,
    MenuItemPopup,
  },

  setup() {},
});
</script>
