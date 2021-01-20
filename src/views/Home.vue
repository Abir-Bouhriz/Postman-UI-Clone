<template>
  <div class="home">
     <v-app>
      <v-row>
        <v-col cols="12" lg="3" >
          <template>
            <requests :requests="requests"/>
          </template>
        </v-col>

        <v-col cols="12" lg="9">
          <template>
            <launchpad :launchpad="launchpad"/>
          </template>

          <div class="mt-10 ml-5">
            <h1 class="mb-4">Good evening!</h1>
            <p class="font-weight-light">Use Launchpad to start something new, pick up where you left off, or explore some resources to help you master Postman.</p>
          </div>

          <v-row>
            <v-col cols="12" lg="6">
              <template>
                <creation :creation="creation"/>
              </template>
            </v-col>

            <v-col cols="12" lg="6">
              <template>
                <postman :postman="postman"/>
              </template>
            </v-col>
          </v-row>
        </v-col>
      </v-row>
    </v-app>
  </div>
</template>

<script>
import Requests from "@/components/Requests.vue";
import Launchpad from "@/components/Launchpad.vue";
import Creation from "@/components/Creation.vue";
import Postman from "@/components/Postman.vue";


export default {
  name: "home",
  components:{
    Requests,
    Launchpad,
    Creation,
    Postman,
  }
}
</script>
