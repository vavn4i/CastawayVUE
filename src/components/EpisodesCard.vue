<template>
  <li class="episodes__card">
    <img
      :src="require('../images/' + episode_data.img)"
      alt=""
      class="episodes__card-img"
    />
    <div class="episodes__card-information card__information">
      <a href="#" class="card__information-description">
        {{ episode_data.description }}
      </a>
      <a href="#" class="card__information-link">
        {{ episode_data.link }}
      </a>
      <h2 class="card__information-title">
        {{ episode_data.title }}
      </h2>
      <p class="card__information-text">
        {{ episode_data.text }}
      </p>
      <button class="card__information-button">
        {{ episode_data.button }}
      </button>
    </div>
  </li>
</template>

<script>
export default {
  name: "EpisodesCard",
  components: {},
  props: {
    episode_data: {
      type: Object,
      default() {
        return {};
      },
    },
  },
  data() {
    return {};
  },
};
</script>

<style lang="scss">
.episodes__card {
  padding: 40px 45px 40px 40px;
  margin-bottom: 60px;
  background: #000000;
  border-radius: 32px;
  display: flex;
  align-items: center;
  &:last-child {
    margin-bottom: 0;
  }
  &-img {
    margin-right: 53px;
  }

  .card__information {
    display: flex;
    flex-direction: column;
    &-description {
      margin-bottom: 48px;
      padding: 0 16px;
      width: 41px;
      font-size: 18px;
      color: #ffffff;
      border-radius: 6px;
      cursor: pointer;
      text-decoration: none;

    }
    &-link {
      margin-bottom: 18px;
      text-decoration: none;
      font-size: 17px;
      color: #118da8;
      cursor: pointer;
      background: #000000;
    }
    &-title {
      margin-bottom: 28px;
      font-size: 64px;
      line-height: 70px;
      letter-spacing: 2.56px;
      color: #ffffff;
      background: #000000;
    }
    &-text {
      margin-bottom: 18px;
      font-size: 22px;
      line-height: 33px;
      color: rgba(255, 255, 255, 0.7);
      background: #000000;
    }
    &-button {
      width: 208px;
      padding: 12px 15px 12px 20px;
      font-size: 18px;
      color: #ffffff;
      background: #118da8;
      border-radius: 6px;
      border: none;
    }
  }
}
.episodes__card:nth-child(2) .card__information .card__information-description {
  width: 106px;
}
</style>
