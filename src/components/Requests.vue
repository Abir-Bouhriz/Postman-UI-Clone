<template>
  <div class="px-3" style="border-right: 1px solid grey; height: 2050px">
    <v-text-field
      outlined
      rounded
      hide-details
      dense
      label="Filter"
      prepend-inner-icon="mdi-magnify"
      single-line
      color="orange darken-3"
      class="pt-2"
    >
    </v-text-field>
    <div class="text-center mt-3">
      <v-btn tile class="px-6" style="border-bottom: 4px solid #ef6c00">
        History
      </v-btn>
      <v-btn tile class="px-6"> Collections </v-btn>
      <v-btn tile class="px-6"> APIs </v-btn>
      <v-divider></v-divider>
    </div>
    <v-switch
      class="ml-5 mb-3"
      v-model="ex11"
      label="Save Responses"
      color="orange darken-3"
      hide-details
    >
    </v-switch>
    <v-divider></v-divider>
    <div class="text-center mt-10 mx-10">
      <p class="body-1 font-weight-bold">You haven't sent any requests</p>
      <p class="body-2 grey--text darken-2--text">
        Any request you send in this workspace will appear here.
      </p>
      <v-btn
        elevation="1"
        color="grey darken-3"
        class="text-capitalize mt-5 py-7 subheading font-weight-bold"
      >
        <v-icon class="mr-1" color="#EF6C00">north_west</v-icon>
        <span class="mr-1 grey--text">Show me how</span>
      </v-btn>
    </div>
  </div>
</template>