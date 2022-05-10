<template>
  <v-app>
    <router-view class="py-16" />
    <v-footer app class="footer d-flex justify-center text-center py-5">
      © 2021 ADVANCED INFO SERVICE PLC. ALL RIGHTS RESERVED.
    </v-footer>
  </v-app>
</template>

<script>

export default {
  name: "App",
};
</script>

<style>
.footer {
  background-color: #B2D235!important;
  color: white!important;
}

</style>
