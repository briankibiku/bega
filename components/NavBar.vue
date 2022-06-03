<template>
  <div>
    <b-navbar toggleable="lg" class="navbar-container">
      <b-navbar-brand href="/">
        <img
          src="~/assets/logo.png"
          alt=""
          class="d-inline-block align-text-top brand-name"
      /></b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
          <b-navbar-nav class="menu">
            <button class="transparent-button" @click="navigateToRankings()">
              <div>About</div>
            </button>
            <button class="transparent-button" @click="navigateToRankings()">
              <div>Contact</div>
            </button>
            <button class="round-white-button" @click="navigateToRankings()">
              <div>Donate</div>
            </button>
          </b-navbar-nav>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>
<style>
/* home route and active route will show in bold as it matches / and /about */
a.nuxt-link-active {
  font-weight: bold;
  color: cyan;
}
/* exact link will show the primary color for only the exact matching link */
a.nuxt-link-exact-active {
  color: #00c58e;
}
.nuxt-link-prefetched {
  color: orangeRed;
}
</style>
