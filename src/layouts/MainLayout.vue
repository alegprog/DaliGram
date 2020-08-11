<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated>
      <q-toolbar>
        <q-btn flat dense round icon="menu" aria-label="Menu" />
        <q-toolbar-title>DaliGram</q-toolbar-title>

        <div>v1.0</div>
      </q-toolbar>
    </q-header>

    <q-footer class="bg-white" elevated>
         <q-tabs 
         class="text-brown-10"
         active-color="primary"
         >
       <q-route-tab
          icon="eva-home-outline"
          to="/"
          />
        <q-route-tab
          icon="eva-camera-outline"
          to="/camera"
          />
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

<style>
.q-tab__icon {
  font-size: 30px;
}
</style>