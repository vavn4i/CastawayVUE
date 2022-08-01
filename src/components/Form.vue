<template>
  <div class="forma container">
    <div class="forma__title">
      <a href="#" class="link"> Email Newsletter </a>
      <h2 class="title">Subscribe for updates</h2>
    </div>
    <form action="" class="form">
      <input placeholder="Name" type="text" class="form__input" />
      <input placeholder="Email" type="text" class="form__input" />
      <button class="form__button">Submit</button>
    </form>
  </div>
</template>

<script>
export default {
  name: "Form",
  components: {},
};
</script>

<style lang="scss">
.forma {
  padding: 60px 60px 75px;
  display: flex;
  background: #000000;
  border-radius: 32px;
  &__title {
    .link {
      font-size: 18px;
      line-height: 27px;
      color: #118da8;
      cursor: pointer;
      text-decoration: none;
      background: #000000;
    }
    .title {
      font-size: 72px;
      line-height: 79px;
      letter-spacing: 2.88px;
      color: #ffffff;
      background: #000000;
    }
  }

  .form {
    display: flex;
    flex-direction: column;
    &__input {
      margin-bottom: 20px;
      padding: 26px 0 25px 19px;
      width: 522px;
      background: #191919;
      border: 1px solid #191919;
      border-radius: 6px;
      cursor: pointer;
      &::placeholder {
        font-size: 24px;
        line-height: 29px;
        color: rgba(255, 255, 255, 0.7);
      }
    }
    &__button {
      padding: 9px 15px 10px 19px;
      width: 87px;
      background: #118da8;
      border-radius: 6px;
      border: none;
      cursor: pointer;
      font-weight: 700;
      font-size: 15px;
      line-height: 29px;
      color: rgba(255, 255, 255, 0.7);
    }
  }
}
</style>
