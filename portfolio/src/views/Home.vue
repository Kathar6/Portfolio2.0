<template>
  <div class="block-photo">
    <div class="blur">
      <img src="/images/oV8NwKAh.jpg" alt="Logo">
      <h1>Mateo Alonso Pabón García</h1>
    </div>
  </div>
  <Nav/>
  <section>
    <p>
      Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur vestibulum dignissim orci id porttitor. Nulla euismod tortor sed erat dapibus, id dapibus nulla congue. Aenean gravida ex id cursus gravida. Nulla ipsum est, suscipit non lacinia ut, vehicula sed felis. Sed euismod tempus enim ut facilisis. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam eleifend nisi eget lobortis egestas. Phasellus lacinia, tortor id maximus laoreet, urna nunc feugiat sem, et gravida justo nisl ac purus. Mauris eget quam orci. Proin varius lorem ultrices, tincidunt ligula non, lacinia tortor.
    
      Ut maximus pharetra urna, et molestie justo rhoncus sed. Mauris non felis ac turpis rhoncus interdum eget ut mauris. Nunc porta velit id dignissim tincidunt. Donec porttitor laoreet elit, aliquet ultricies metus tristique eget. Nullam maximus, lorem non vehicula molestie, orci est convallis libero, efficitur pharetra purus quam eu neque. Proin porttitor blandit lectus ut facilisis. Praesent bibendum, erat a mollis faucibus, augue orci elementum sapien, luctus fringilla sem ex quis est. Praesent semper diam in diam mattis, sed ultrices elit fermentum. Vivamus aliquet pharetra urna.
    </p>

    <h1>Projects</h1>

    <p>
      Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur vestibulum dignissim orci id porttitor. Nulla euismod tortor sed erat dapibus, id dapibus nulla congue. Aenean gravida ex id cursus gravida. Nulla ipsum est, suscipit non lacinia ut, vehicula sed felis. Sed euismod tempus enim ut facilisis. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam eleifend nisi eget lobortis egestas. Phasellus lacinia, tortor id maximus laoreet, urna nunc feugiat sem, et gravida justo nisl ac purus. Mauris eget quam orci. Proin varius lorem ultrices, tincidunt ligula non, lacinia tortor.
    
      Ut maximus pharetra urna, et molestie justo rhoncus sed. Mauris non felis ac turpis rhoncus interdum eget ut mauris. Nunc porta velit id dignissim tincidunt. Donec porttitor laoreet elit, aliquet ultricies metus tristique eget. Nullam maximus, lorem non vehicula molestie, orci est convallis libero, efficitur pharetra purus quam eu neque. Proin porttitor blandit lectus ut facilisis. Praesent bibendum, erat a mollis faucibus, augue orci elementum sapien, luctus fringilla sem ex quis est. Praesent semper diam in diam mattis, sed ultrices elit fermentum. Vivamus aliquet pharetra urna.
    </p>
  </section>
  <Footer/>
</template>

<script>
// @ is an alias to /src
import Nav from "@/components/Nav.vue";
import Footer from "@/components/Footer.vue"

export default {
  name: "Home",
  components: {
    Nav,
    Footer
  }
};
</script>

<style lang="scss" scoped>
  .block-photo {
    width: 100%;
    min-height: 60vh;
    max-height: 70vh;
    background-image: url("../../public/images/main_background.jpg");
    background-size: cover;
    & .blur{
      display: grid;
      grid-template-rows: 1fr 1fr;
      width:100%;
      min-height: 60vh;
      max-height: 70vh;
      backdrop-filter: blur(2px);
      & img {
        grid-row: 0/1;
        width: 10%;
        margin: 5% auto;
        border: 5px solid #eee;
        border-radius: 100%;
        box-shadow: 0px 0px 10px 3px #616161;
      }
      & h1 {
        color: white;
      }
    }
  }
  section {
    padding: 0 2%;
    & h1 {
      margin: 2% 0;
    }
  }
</style>
