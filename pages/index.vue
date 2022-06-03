<template>
  <div>
    <NavBar />
    <div class="d-flex flex-direction-row">
      <div class="container">
        <div class="row align-items-start">
          <div class="col">
            <div class="landing-text-black">
              <p class="detail">
                Feel like <span class="name">giving up</span> on
                <span class="name">life?</span>
              </p>
              <p class="subdetail">
                Give us a <span class="subname">chance </span> to talk to you,
                <span class="subname">everything will be alright</span>
              </p>
            </div>
            <div>
              <button class="round-pink-button" @click="navigateToContact()">
                <div>Get counselling</div>
              </button>
            </div>
          </div>
          <div class="col">
            <div class="listen-container"></div>
          </div>
        </div>
      </div>
    </div>
    <Footer />
  </div>
</template>

<script>
import NavBar from "../components/NavBar.vue";
import Footer from "../components/Footer.vue";
export default {
  methods: {
    navigateToContact() {
      return this.$router.push("/");
    },
  },
  components: { NavBar, Footer },
};
</script>

<style>
p.detail {
  color: #4c4c4c;
  font-weight: bold;
  font-size: 1em;
  padding-inline: 40px;
  text-align: left;
}
span.name {
  color: #f65578;
  font-weight: bolder;
  font-size: 1em;
}
p.subdetail {
  color: #4c4c4c;
  font-weight: bold;
  font-size: 0.5em;
  padding-inline: 40px;
  text-align: left;
}
span.subname {
  color: #f65578;
  font-weight: bolder;
}
</style>
