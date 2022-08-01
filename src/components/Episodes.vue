<template>
  <div class="episodes container">
    <div class="episodes__block">
      <h2 class="episodes__title">Latest episodes</h2>
      <button class="episodes__button">View all episodes</button>
    </div>
    <ul class="episodes__cards">
      <EpisodesCard 
      v-for="episodes__card in episodes__cards"
      :key="episodes__card.link"
      :episode_data="episodes__card"
      />
    </ul>
  </div>
</template>

<script>
import EpisodesCard from "./EpisodesCard.vue";

export default {
  name: "Episodes",
  components: {
    EpisodesCard,
  },
  props: {},
  data() {
    return {
      episodes__cards: [
        {
          img: "audioGear.png",
          description: "Gear",
          link: "Episode 3",
          title: "Should you get outboard audio gear?",
          text: "Is hardware really worth it when it comes to podcasting? The answer is...it depends. Here’s our reasons on why you might want to consider picking something up.",
          button: "View Episode Details",
        },
        {
          img: "mic.png",
          description: "Tips & Tricks",
          link: "Episode 2",
          title: "Mic tricks to take you to the next level",
          text: "Stop rolling with those default settings on your mic. These small tweaks will take you from sounding good to great.",
          button: "View Episode Details",
        },
        {
          img: "bestMicrophone.png",
          description: "Gear",
          link: "Episode 1",
          title: "The best microphone under $200",
          text: "With so many microphones on the market, how are you supposed to know what’s the best? Take a look at our top picks.",
          button: "View Episode Details",
        },
      ],
    };
  },
  computed: {},
};
</script>

<style lang="scss">
.episodes {
  padding-top: 93px;
  margin-bottom: 260px;
  &__cards{
    margin-bottom: 260px;
  }
  &__block {
    margin-bottom: 66px;
    display: flex;
    justify-content: space-between;

    .episodes__title {
      font-weight: 400;
      font-size: 64px;
      color: #ffffff;
    }
    .episodes__button {
      padding: 12px 15px 12px 20px;
      height: 51px;
      background: #118da8;
      border-radius: 6px;
      font-weight: 400;
      font-size: 17px;
      line-height: 27px;
      color: #ffffff;
      cursor: pointer;
      border: none;
    }
  }
}
</style>
