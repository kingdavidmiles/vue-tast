<template>
  <div style="background-color: #1a3c59; color: white" class="pt-5">
    <v-row>
      <v-col md="2" sm="12"></v-col>
      <v-col md="8" sm="12">
        <div class="text-center pt-5 pb-5">STAY UP TO DATE WITH SABA IP</div>
        <div class="pb-5">
          Fill out the form below to receive event and news alerts.
        </div>
        <v-form class="pt-5 pb-5">
          <v-row class="mx-sm-5">
            <v-col md="6" sm="12">
              <label>Full Name</label>
              <v-text-field label="full name" variant="solo"></v-text-field>
            </v-col>
            <v-col md="6">
              <label>Email</label>
              <v-text-field label="Email" variant="solo"></v-text-field>
            </v-col>
            <v-col md="6">
              <label>Select Your Country</label>
              <v-select
                label="Select"
                :items="[
                  'California',
                  'Colorado',
                  'Florida',
                  'Georgia',
                  'Texas',
                  'Wyoming',
                ]"
                variant="solo"
              ></v-select>
            </v-col>
          </v-row>
          <div class="pt-5 pb-3 mx-sm-5">
            <v-btn variant="tonal" size="large" class="button-color">
              subscribe
            </v-btn>
          </div>
        </v-form>
      </v-col>
      <v-col md="2"></v-col>
    </v-row>
    <!--  -->
  </div>
  <div>
    <v-row>
      <v-col md="2" sm="12"></v-col>
      <v-col md="8" sm="12" >
        <v-sheet class="d-flex mb-6">
          <v-sheet class="ma-2 pa-2 me-auto">
            <div>
              Privacy Policy | All Rights Reserved | Designed by Beirut in
            </div>
          </v-sheet>
          <v-sheet class="ma-2 pa-2">
            <span class="mr-4"><v-icon icon="mdi-linkedin"></v-icon></span>
            <span class="mr-2"><v-icon icon="mdi-twitter"></v-icon></span>
            <span class="ml-4"><v-icon icon="mdi-email-outline"></v-icon></span>
          </v-sheet>
        </v-sheet>
      </v-col>
      <v-col md="2"></v-col>
    </v-row>
  </div>
</template>
