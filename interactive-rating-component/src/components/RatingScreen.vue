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
          <input id="1" type="radio" name="rating" value="1" class="hidden" />
          <label class="rating-icon content-icon" for="1">1</label>
          <input id="2" type="radio" name="rating" value="2" class="hidden" />
          <label class="rating-icon content-icon" for="2">2</label>
          <input id="3" type="radio" name="rating" value="3" class="hidden" />
          <label class="rating-icon content-icon" for="3">3</label>
          <input id="4" type="radio" name="rating" value="4" class="hidden" />
          <label class="rating-icon content-icon" for="4">4</label>
          <input id="5" type="radio" name="rating" value="5" class="hidden" />
          <label class="rating-icon content-icon" for="5">5</label>
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
  border-radius: 30px;
  background-image: radial-gradient(circle at 50% 0, #232a34, #181e27 89%);
}

.content {
  font-family: "Overpass", sans-serif;
  display: flex;
  flex-direction: column;
  &_container {
    max-width: 340px;
    margin: 32px 40px 32px 32px;
  }
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
  &-heading {
    color: #fff;
    font-size: 1.75rem;
    font-weight: 700;
    margin-top: 30px;
    margin-bottom: 7px;
  }
  &-description {
    color: #969fad;
    font-size: 0.938rem;
    line-height: 1.5rem;
    margin-top: 0px;
    margin-bottom: 24px;
  }
}

.rating {
  &_container {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    margin-bottom: 32px;
  }
  &-icon {
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 1rem;
    line-height: 1.5rem;
    color: #7c8798;
    cursor: pointer;
    &:hover {
      background-color: #fc7614;
      color: #fff;
    }
  }
  &-button {
    width: 341px;
    height: 45px;
    padding: 11px 138px 11px 137px;
    border-radius: 22.5px;
    background-color: #fc7614;
    color: #fff;
    border: 0px;
    font-size: 0.938rem;
    font-weight: 700;
    letter-spacing: 2px;
    text-transform: uppercase;
  }
}
input:checked + .rating-icon {
  background-color: #fc7614;
  color: #fff;
}
</style>
