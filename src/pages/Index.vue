<template>
  <q-page
    class="page-width flex flex-center q-mx-auto bg-pallette-white q-mt-sm q-py-xxl"
  >
    <div class="w-full">
      <header class="text-center row justify-end contact-page">
        <div class="col padding-r-100px"></div>
        <div class="col">
          <h2 class="font-black font-gray-text-darker q-my-md">Contact Us</h2>
          <h5 class="font--yellow font-black q-my-none">
            Feel free to send us a message
          </h5>
        </div>
      </header>

      <div class="row items-stretch contact-page q-mt-xl">
        <div class="col contact-page-left padding-r-100px">
          <div class="w-full">
            <h3 class="q-mb-md text-center font-black font-gray-text-darker">
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

          <div
            class="q-mt-xl q-pa-xxl border-radius-16px bg-pallette-gray-warmer text-center"
          >
            <h3 class="font-black q-mt-none q-mb-none font-gray-text-darker">
              Schedule <br />
              a live demo
            </h3>
            <q-btn
              class="q-mt-lg bg-white text-capitalize font-gray-text-darker font-black"
              bg-color="#"
              flat
              size="1rem"
              >Schedule</q-btn
            >
          </div>
        </div>
        <div class="col">
          <div
            class="q-mt-xl q-pa-xl border-radius-16px bg-pallette-gray-warmer text-center"
          >
            <q-form>
              <div class="q-mt-lg">
                <p
                  class="q-mb-none text-left text-bold font-size-14px font-gray-text-dark"
                >
                  Your Name:*
                </p>
                <q-input
                  standout
                  outlined
                  placeholder="John..."
                  bg-color="white"
                  class="font-size-16px"
                  input-class="q-py-none"
                />
              </div>
              <div class="q-mt-lg">
                <p
                  class="q-mb-none text-left text-bold font-size-14px font-gray-text-dark"
                >
                  Your E-mail:*
                </p>
                <q-input
                  standout
                  outlined
                  placeholder="Your email address ...@..."
                  bg-color="white"
                  class="font-size-16px"
                  input-class="q-py-none"
                />
              </div>
              <div class="q-mt-lg">
                <p
                  class="q-mb-none text-left text-bold font-size-14px font-gray-text-dark"
                >
                  Your Message:*
                </p>
                <q-input
                  standout
                  type="textarea"
                  outlined
                  placeholder="John..."
                  bg-color="white"
                  class="font-size-16px"
                  input-class="q-py-none"
                />
              </div>
              <p class="q-mt-lg">
                This site is protected by reCAPTCHA and the Google Privacy
                Policy and Terms of Service apply.
              </p>

              <q-btn
                label="Send"
                no-caps
                flat
                size="1rem"
                text-color="white"
                class="full-width no-shadow bg-pallette-yellow text-bold"
              />
            </q-form>
          </div>
        </div>
      </div>
    </div>
  </q-page>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "PageIndex",
});
</script>
