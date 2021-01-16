<template>
  <div class="home">
    <v-app>
      <v-row>

        <v-col cols="12" lg="3" >
          <div class="px-3" style="background:#212121; height: 750px;">
          <v-text-field label="Filter" outlined rounded hide-details dense prepend-inner-icon="mdi-magnify" single-line color="orange darken-3" class="pt-2" ></v-text-field>
        <div class="text-center mt-3">
          <v-btn tile class="px-7" style="border-bottom: 4px solid #EF6C00">History </v-btn>
          <v-btn tile class="px-7">Collections </v-btn>
          <v-btn tile class="px-7">APIs </v-btn>
          <v-divider></v-divider>
          </div>
      <v-switch class="ml-5 mb-3"
              v-model="ex11"
              label="Save Responses"
              color="orange darken-3"
              value="orange darken-3"
              hide-details
            ></v-switch>
            <v-divider></v-divider>
            <div class="text-center mt-10 mx-10">
          <p class="body-1 font-weight-bold">You haven't sent any requests</p>
          <p class="body-2 grey--text darken-2--text">Any request you send in this workspace will appear here.</p>
          <v-btn elevation="1" color="grey darken-3" class="text-capitalize mt-5 py-7 subheading font-weight-bold " >
            <v-icon class="mr-1" color="#EF6C00">north_west</v-icon>
            <span class="mr-1 grey--text ">Show me how</span>
        </v-btn>
        </div>
        </div>
        </v-col>

        <v-col cols="12" lg="9">

        </v-col>
      </v-row>
    </v-app>
  </div>
</template>

<script>
// @ is an alias to /src


export default {
  name: 'Home',
 
}
</script>
