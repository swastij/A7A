<template>
  <div class="home">
    <navbar />
    <hero />
    <arrow />
    <aboutus />
    <takeaction />
    <feature />
    <loremipsum />
    <jointhemovement />
    <foot />
  </div>
</template>

<script>
// @ is an alias to /src
import navbar from "../components/navbar.vue";
import hero from "../components/hero.vue";
import arrow from "../components/arrow.vue";
import aboutus from "../components/aboutus.vue";
import takeaction from "../components/takeaction.vue";
import feature from "../components/feature.vue";
import loremipsum from "../components/loremipsum.vue";
import jointhemovement from "../components/jointhemovement.vue";
import foot from "../components/foot.vue";

export default {
  name: "Home",
  components: {
    navbar,
    hero,
    arrow,
    aboutus,
    takeaction,
    feature,
    loremipsum,
    jointhemovement,
    foot
  }
};
</script>
<style>
.home {
  width: 87%;
  max-width: 87%;
  padding: 2%;
  height: 100%;
  margin: auto;
  /* position: relative; */
}
</style>
