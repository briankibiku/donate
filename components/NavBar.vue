<template>
  <div>
    <b-navbar
      toggleable="lg"
      fixed="top"
      type="light"
      variant="light"
      style="padding-inline: 4vw"
    >
      <b-navbar-brand href="/">
        <img
          src="~/assets/images/logo_three.png"
          alt=""
          width="190"
          height="80"
          class="d-inline-block align-text-top"
      /></b-navbar-brand>
      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
      <b-collapse id="nav-collapse" is-nav>
        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
          <b-navbar-nav class="menu">
            <b-nav-item href="/" class="menu">Home</b-nav-item>
            <b-nav-item href="/about" class="menu">About</b-nav-item>
            <b-nav-item href="/programs">Programs</b-nav-item>
            <b-nav-item href="/partners">Partners</b-nav-item>
            <b-nav-item href="/contact">Contact</b-nav-item>
            <b-button
              @click=""
              href="/blood-donation"
              style="width: 140px; background-color: #c82333; border: none"
              >Donate</b-button
            >
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
