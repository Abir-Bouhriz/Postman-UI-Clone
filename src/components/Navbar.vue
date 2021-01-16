<template>
 <v-app-bar app flat height="60">
        <v-btn dense elevation="2" color="orange darken-3" class="text-capitalize mr-3 subheading font-weight-bold " >
            <v-icon class="mr-2 ml-n2">add_box</v-icon>
            <span class="mr-n2">New</span>
        </v-btn>
        <v-btn elevation="2" color="grey darken-3" class="text-capitalize mr-3 subheading font-weight-bold " >Import</v-btn>
        <v-btn elevation="2" color="grey darken-3" class="text-capitalize mr-3 subheading font-weight-bold " >Runner</v-btn>
        <v-btn elevation="2" color="grey darken-3" class="text-capitalize mr-3 subheading font-weight-bold " >
            <v-icon class="mr-1 ml-n2">post_add</v-icon>
            <v-icon class="mr-n2">arrow_drop_down</v-icon>
        </v-btn>

        <v-spacer></v-spacer>

        <v-btn text  class="text-capitalize mr-5 subheading font-weight-bold " >
            <v-icon class="mr-2">dashboard</v-icon>
            <span class="mr-2">My Work Space</span>
            <v-icon>arrow_drop_down</v-icon>
        </v-btn>
        <v-btn elevation="2" color="grey darken-3" class="text-capitalize mr-5 subheading font-weight-bold " >
            <v-icon class="mr-2 ml-n2">person_add_alt_1</v-icon>
            <span class="mr-n2">Invite</span>
        </v-btn>
    
      <v-spacer></v-spacer>
        <v-btn fab small class="mr-2 orange darken-3" >
            <v-icon > autorenew </v-icon>
        </v-btn>
        <v-btn fab small class="mr-2" >
            <v-icon > wifi_tethering </v-icon>
        </v-btn>
        <v-btn fab small class="mr-2" >
            <v-icon > settings </v-icon>
        </v-btn>
        <v-btn fab small class="mr-2" >
            <v-icon > notifications</v-icon>
        </v-btn>
        <v-btn fab small class="mr-2" >
            <v-icon > favorite </v-icon>
        </v-btn>
        <v-btn fab small class="mr-2 teal lighten-2" >
            <v-icon > account_tree </v-icon>
        </v-btn>
        <v-btn elevation="2" color="grey darken-3" class="text-capitalize  subheading font-weight-bold " >
            <span class="mr-1 ">Upgrade</span>
            <v-icon class="mr-n2">arrow_drop_down</v-icon>
        </v-btn>
      
          
  </v-app-bar>
</template>

<script>
export default {
    
}
</script>