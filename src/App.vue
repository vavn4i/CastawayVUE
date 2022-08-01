<template>
  <div id="app">
    <Header />
    <Baner />
    <Episodes /> 
    <Author /> 
    <Form /> 
    <Reviews />
    <Review /> 
    <Footer />   
  </div>
</template>

<script>
  import Header from './components/Header.vue';
  import Baner from './components/Baner.vue';
  import Episodes from './components/Episodes.vue';
  import Author from './components/Author.vue';
  import Form from './components/Form.vue';
  import Reviews from './components/Reviews.vue';
  import Review from './components/Review.vue';
  import Footer from './components/Footer.vue';



export default {
  name: 'App',
  components: {
    Header,
    Baner,
    Episodes,
    Author,
    Form,
    Reviews,
    Review,
    Footer
  }
}
</script>

<style >

</style>
