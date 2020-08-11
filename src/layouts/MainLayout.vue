<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated class="bg-white text-brown-10">
      <q-toolbar class="constrain">
        <q-btn flat round icon="eva-camera-outline large-screen-only q-mr-sm" size="18px" dense to="/camera" />
        <q-separator vertical spaced class="large-screen-only" />
        <q-toolbar-title class="text-grand-hotel text-bold">DaliGram</q-toolbar-title>
        <q-btn flat round icon="eva-home-outline large-screen-only" size="18px" dense to="/" />
      </q-toolbar>
    </q-header>

    <q-footer class="bg-white small-screen-only" elevated>
      <q-tabs class="text-brown-10" active-color="primary">
        <q-route-tab icon="eva-home-outline" to="/" />
        <q-route-tab icon="eva-camera-outline" to="/camera" />
      </q-tabs>
    </q-footer>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
export default {
  name: "MainLayout",
  data() {
    return {};
  },
};
</script>

<style lang="scss">
.q-toolbar {
   @media (min-width: $breakpoint-sm-min) {
  height: 4rem;
   }
}
.q-tab__icon {
  font-size: 30px;
}
.q-toolbar__title {
   @media (max-width: $breakpoint-xs-max) {
  text-align: center;
   }
}
.text-grand-hotel {
  font-size: 35px;
}
</style>