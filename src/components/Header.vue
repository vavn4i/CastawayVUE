<template>
  <header class="header">
    <img src="../images/logo.png" alt="" class="header__img" />
    <ul class="header__list">
      <li class="header__list-link">
        <a href="#" class="link">Home</a>
      </li>
      <li class="header__list-link">
        <a href="#" class="link">Episodes</a>
      </li>
      <li class="header__list-link">
        <a href="#" class="link">About</a>
      </li>
      <li class="header__list-link">
        <a href="#" class="link">Contact</a>
      </li>
    </ul>
  </header>
</template>

<script>
export default {
  name: "Header",
  components: {},
};
</script>

<style lang="scss">
  .header{
    padding: 43px 70px 43px 50px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    &__img{
      width: 160px;
      height: 33px;
    }
    &__list{
      display: flex;
      &-link{
        margin-right:40px ;
        list-style: none;
        &:last-child{
          margin-right: 0;
        }
        .link{
          text-decoration: none;
          font-weight: 400;
          font-size: 17px;
          line-height: 27px;
          color: #FFFFFF;
          cursor: pointer;
          &:hover{
            color: #118DA8;
          }
          
        }
      }
    }
  }
</style>
