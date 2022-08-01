<template>
  <div class="baner container">
    <img src="../images/baner.png" alt="" class="baner__img" />
    <div class="informations ">
      <h1 class="title">Take your podcast to the <span>next</span> <b>level</b></h1>
      <span> Listen on </span>
      <ul class="baner__list">
        <li class="baner__item">
          <a href="#">
            <img src="../images/spotify.svg" alt="" class="link__social" />
          </a>
        </li>
        <li class="baner__item">
          <a href="#">
            <img src="../images/spotufyRed.svg" alt="" class="link__social" />
          </a>
        </li>
        <li class="baner__item">
          <a href="#">
            <img src="../images/sky.svg" alt="" class="link__social" />
          </a>
        </li>
        <li class="baner__item">
          <a href="#">
            <img src="../images/podcasts.svg" alt="" class="link__social" />
          </a>
        </li>
        <li class="baner__item">
          <a href="#">
            <img src="../images/radio.svg" alt="" class="link__social" />
          </a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "Baner",
  components: {},
};
</script>

<style lang="scss">
.baner{
  padding-top: 40px;
  display: flex;
  align-items: center;
 
 
  &__img{
    margin-right: 60px;
    width: 650px;
    height: 873px;
  }

  .informations{
    .title{
      margin-bottom: 90px;
      font-weight: 400;
      font-size: 70px;
      color: #FFFFFF;
      span{
        font-weight: 400;
        font-size: 75px;
        color: #FFFFFF;
      }
    }
    span{
      font-weight: 400;
      font-size: 15px;
      color: #FFFFFF;
    }
    .baner__list{
      margin-top: 15px;
      display: flex;
      .baner__item{
        margin-right: 17px;
        cursor: pointer;
        &:last-child{
          margin-right: 0;
        }
        .link__social{
          width: 32px;
          height: 32px;
        }
      }

    }
  }
}

</style>
