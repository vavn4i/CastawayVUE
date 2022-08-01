<template>
  <div class="author container">
    <div class="author__information">
      <a href="#" class="author__information-more">
        <img src="../images/arrow.png" alt=""  />
      </a>
      <a href="#" class="author__information-link"> Meet your host </a>
      <h2 class="author__information-name">Jacob Paulaner</h2>
      <p class="author__information-about-me">
        Jacob has a background in audio engineering, and has been podcasting since the early days.
      </p>
      <p class="author__information-about-me">
        He’s here to help you level up your game by sharing everything he’s learned along the way.
      </p>
    </div>
    <img src="../images/Jacob.png" alt="" class="author__img">
  </div>
</template>

<script>
export default {
  name: "Author",
  components: {},
};
</script>

<style lang="scss">
  .author{
    display: flex;
    align-items: center;
    &__img{
          margin-bottom: 200px;
    }
    &__information{
      margin-right: 94px;
      display: flex;
      flex-direction: column;
      &-more{
        margin-bottom: 20px;
        width: 112px;
      }
      &-link{
        text-decoration: none;
        font-size: 18px;
        line-height: 27px;
        color: #118DA8;
      }
      &-name{
        margin-bottom: 28px;
        font-size: 65px;
        line-height: 79px;
        letter-spacing: 2.88px;
        color: #FFFFFF;
      }
      &-about-me{
        margin-bottom: 33px;
        font-size: 22px;
        line-height: 33px;
        color: rgba(255, 255, 255, 0.7);
        &:last-child{
          margin-bottom: 0;
        }
      }
    }
  }

</style>
