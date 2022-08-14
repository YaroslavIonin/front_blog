<template>
  <div>
    <Navbar />
    <Slider />
    <div>
      <Nuxt />
    </div>
    <Footer />
  </div>
</template>


<script>
import Navbar from "~/components/Navbar";
import Slider from "~/components/Slider";
import Footer from "~/components/Footer";

export default {
  components: {
    Navbar,
    Footer,
    Slider,
  },
  head() {
    return {
      link: [
        { rel: "canonical", href: `http://localhost:3000${this.$route.path}`}
      ]
    }
  },
};
</script>

<style>

</style>
