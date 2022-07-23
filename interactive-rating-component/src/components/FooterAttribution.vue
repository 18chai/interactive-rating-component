<template>
  <div class="attribution">
    Challenge by&nbsp;
    <a
      class="attribution-link"
      href="https://www.frontendmentor.io?ref=challenge"
      target="_blank"
      >Frontend Mentor</a
    >. Coded by&nbsp;
    <a class="attribution-link" href="https://kolektivum.com">Radek Berka</a>.
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

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.attribution {
  display: flex;
  flex-direction: row;
  color: #969fad;
  &-link {
    color: #fc7614;
  }
}
</style>
