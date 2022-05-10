<template>
  <v-container
    transition="expand-x-transition"
    fluid
    class="d-flex flex-column justify-center align-center my-auto"
  >
    <v-img
      src="https://www.ais.th/vaccinesforthais/images/vaccines-logo.png"
    ></v-img>
    <h1>เชื่อมต่อ ช่วยเหลือ เพื่อคนไทยสู้ภัยโควิด</h1>
    <h2>Connecting All Thais in the Fight Agianst COVID</h2>
    <v-img
      contain
      src="https://www.ais.th/vaccinesforthais/images/vaccine28-04-2022.png"
      max-width="900"
    ></v-img>
    <v-btn rounded color="#B2D235" href="/login" class="text-capitalize hover-darker pa-6 text-h5 my-8"
      >ลงทะเบียนจอคิว - Register</v-btn
    >
  </v-container>
</template>

<style scoped>
.hover-darker:hover {
  background-color: black !important;
  color: #b2d235 !important;
}
</style>
