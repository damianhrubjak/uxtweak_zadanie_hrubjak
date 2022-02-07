<template>
  <q-page
    class="page-width flex flex-center q-mx-auto bg-pallette-white q-mt-sm"
  >
    <div class="w-full contact-page-grid contact-page-padding page-wrapper">
      <div class="grid-spacer"></div>
      <header class="text-center justify-end">
        <Banner
          heading="Contact Us"
          subHeading="Feel free to send us a message"
        />
      </header>

      <div class="contact-page-left">
        <div class="w-full">
          <h3
            class="q-mb-md q-mt-none text-center font-black font-gray-text-darker"
          >
            <span class="font--yellow">Bee</span>p Us
          </h3>
          <a
            href="#"
            class="font--yellow text-bold font-size-16px text-center block"
            >info@uxtweak.com</a
          >
          <div class="text-center q-mt-md">
            <p
              class="font-black q-mb-none font-gray-text-darker font-size-16px"
            >
              Office
            </p>
            <p
              class="q-mb-none font-gray-text-darker font-medium font-size-16px"
            >
              UXtweak j.s.a., Obchodna 58, 811 06 Bratislava <br />
              Slovakia (European Union)
            </p>
          </div>
        </div>

        <ScheduleLiveDemo />
      </div>
      <div
        class="contact-form-wrapper q-pa-xl border-radius-16px bg-pallette-gray-warmer text-center q-mx-auto"
      >
        <ContactForm />
      </div>
    </div>
  </q-page>
</template>

<script>
import { defineComponent } from "vue";
import ContactForm from "../components/contact-form";
import Banner from "../components/banner";
import ScheduleLiveDemo from "src/components/schedule-live-demo.vue";

export default defineComponent({
  name: "PageIndex",

  components: {
    ContactForm,
    Banner,
    ScheduleLiveDemo,
  },
});
</script>
