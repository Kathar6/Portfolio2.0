<template>
  <div class="about">
    <h1>This is an about page</h1>
    <Nav/>
    <Footer/>
  </div>
</template>

<script>
import Nav from "@/components/Nav.vue";
import Footer from "@/components/Footer.vue"
export default {
  name: "About",
  components: {
    Nav,
    Footer
  }
}
</script>