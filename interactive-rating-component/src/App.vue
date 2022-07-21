<template>
  <div class="main">
    <RatingScreen />
    <FooterAttribution />
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import RatingScreen from "./components/RatingScreen.vue";

export default defineComponent({
  name: "App",
  components: {
    RatingScreen,
    FooterAttribution,
  },
});

import "./styles/main.scss";
import FooterAttribution from "./components/FooterAttribution.vue";
</script>
