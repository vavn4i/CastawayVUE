<template>
  <li class="review ">
    <ul class="list__star">
      <li class="star__item">
        <img :src=" require('../images/' + review_data.img) " alt="" class="star__img" />
      </li>
      <li class="star__item">
        <img :src=" require('../images/' + review_data.img) " alt="" class="star__img" />
      </li>
      <li class="star__item">
        <img :src=" require('../images/' + review_data.img) " alt="" class="star__img" />
      </li>
      <li class="star__item">
        <img :src=" require('../images/' + review_data.img) " alt="" class="star__img" />
      </li>
      <li class="star__item">
        <img :src=" require('../images/' + review_data.img) " alt="" class="star__img" />
      </li>
    </ul>
    <p class="comment">
        {{review_data.comment}}
    </p>
    <span class="comment__author">
        {{review_data.author}}
    </span>
  </li>
</template>

<script>
export default {
  name: "Review",
  components: {},
    props:{
    review_data: {
      type:Object,
      default(){
        return{}
      }
    }
  },
  data() {
    return{}
  },
};
</script>


<style lang="scss"> 
    .review{
        margin-right: 16px;
        margin-bottom: 16px;
        padding: 54px 56px 51px 50px;
        background: #000000;
        border-radius: 32px;
        width: 316px;
        &:nth-child(3n){
            margin-right: 0;
        }
        .list__star{
            margin-bottom: 21px;
            display: flex;
            background: #000000;
            .star__item{
                margin-right: 5px;
                background: #000000;
                &:last-child{
                    margin-right: 0;
                }
            }
        }
        .comment{
            margin-bottom: 19px;
            font-size: 36px;
            line-height: 43px;
            color: #FFFFFF;
            background: #000000;
            &__author{
                font-size: 24px;
                line-height: 29px;
                color: rgba(255, 255, 255, 0.7);
            }
        }


    }

</style>
