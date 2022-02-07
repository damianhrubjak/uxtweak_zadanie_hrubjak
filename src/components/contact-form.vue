<template>
  <q-form>
    <div class="">
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
      This site is protected by
      <a href="" class="font--yellow">reCAPTCHA</a> and the Google Privacy
      Policy and <a href="" class="font--yellow">Terms of Service apply</a>.
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
</template>

<script>
export default {
  setup() {},
};
</script>

<style></style>
