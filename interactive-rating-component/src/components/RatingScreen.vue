<template>
  <div class="rating_box">
    <div class="content content_container">
      <div class="content-icon">
        <img
          class="content-icon_image"
          src="../assets/star.svg"
          alt="Star shape icon in dark orange color"
        />
      </div>
      <h1 class="content-heading">How did we do?</h1>
      <p class="content-description">
        Please let us know how we did with your support request. All feedback is
        appreciated to help us improve our offering!
      </p>
      <form class="content-rating">
        <div class="rating rating_container">
          <div class="rating-icon content-icon">1</div>
          <div class="rating-icon content-icon">2</div>
          <div class="rating-icon content-icon">3</div>
          <div class="rating-icon content-icon">4</div>
          <div class="rating-icon content-icon">5</div>
        </div>
        <div class="rating content-submit">
          <button class="rating-button" type="submit">Submit</button>
        </div>
      </form>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "RatingScreen",
  props: {
    msg: String,
  },
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.rating_box {
  margin: auto;
  width: 412px;
  height: 416px;
  padding: 2rem;
  border-radius: 30px;
  background-image: radial-gradient(circle at 50% 0, #232a34, #181e27 89%);
}

.content {
  display: flex;
  flex-direction: column;
  &-icon {
    display: flex;
    width: 3rem;
    height: 3rem;
    background-color: #262e38;
    border-radius: 50%;
    &_image {
      width: 1rem;
      height: 1rem;
      align-self: center;
      margin: auto;
    }
  }
}

.rating {
  &_container {
    display: flex;
    flex-direction: row;
  }
}
</style>
