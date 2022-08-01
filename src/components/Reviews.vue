<template>
  <ul class="reviews container">
    <Review
      v-for="review__card in reviews__cards"
      :key="review__card.author"
      :review_data="review__card"
    />
  </ul>
</template>

<script>
import Review from "./Review.vue";

export default {
  name: "Reviews",
  components: {
    Review,
  },
  props: {},
  data() {
    return {
      reviews__cards: [
        {
          img: "star.svg",
          comment: "I can’t recommend this podcast enough",
          author: "Betty Lacey",
        },
        {
          img: "star.svg",
          comment: "Jacob is the best in the business",
          author: "Adam Driver",
        },
        {
          img: "star.svg",
          comment: "A wealth of audio knowledge",
          author: "Marcus Brown",
        },
        {
          img: "star.svg",
          comment: "Every episode is a gem!",
          author: "Jessica Knowl",
        },
        {
          img: "star.svg",
          comment: "Whoa whoa, let me take some notes!",
          author: "Scott Adams",
        },
        {
          img: "star.svg",
          comment: "I’ve upped my game considerably since I started listening",
          author: "Steven Blast",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
.reviews {
  padding-top: 200px;
  padding-bottom: 184px;
  display: flex;
  flex-wrap: wrap;
}
</style>
