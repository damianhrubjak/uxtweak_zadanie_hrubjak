<template>
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
      <div class="popup-content">
        <div class="item w-full">
          <p class="q-mb-none font-black">Contact Form</p>
          <p class="q-mb-none text-sm">Feel free to send us message</p>
        </div>
        <div class="item w-full">
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
</template>

<script>
import { defineComponent } from "vue";
import MenuItem from "./menu-item";
import MenuItemPopup from "./menu-item-popup";

export default defineComponent({
  components: {
    MenuItem,
    MenuItemPopup,
  },
});
</script>

<style></style>
