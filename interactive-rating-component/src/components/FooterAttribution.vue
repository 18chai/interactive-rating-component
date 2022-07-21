<template>
  <div class="attribution">
    Challenge by
    <a href="https://www.frontendmentor.io?ref=challenge" target="_blank"
      >Frontend Mentor</a
    >. Coded by <a href="#">Your Name Here</a>.
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "FooterAttribution",
  props: {
    msg: String,
  },
});
</script>
