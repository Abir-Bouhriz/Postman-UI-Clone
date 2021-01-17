<template>
  <div class="home">
    <v-app>
      <v-row>
        <v-col cols="12" lg="3" >
          <div class="px-3" style="background:#212121; border-right:1px solid grey; height: 850px;">
            <v-text-field 
              outlined rounded hide-details dense 
              label="Filter" 
              prepend-inner-icon="mdi-magnify" 
              single-line color="orange darken-3" 
              class="pt-2" >
            </v-text-field>
            <div class="text-center mt-3">
              <v-btn tile class="px-6" style="border-bottom: 4px solid #EF6C00">
                History 
              </v-btn>
              <v-btn tile class="px-6">
                Collections 
              </v-btn>
              <v-btn tile class="px-6">
                APIs 
              </v-btn>
              <v-divider></v-divider>
            </div>
            <v-switch
              class="ml-5 mb-3"
              v-model="ex11"
              label="Save Responses"
              color="orange darken-3"
              hide-details>
            </v-switch>
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
          <v-app-bar class="mx-n3" style="border-bottom:1px solid grey;">
            
              <v-btn elevation="1" color="grey darken-3">
                <span class="text-capitalize">Launchpad</span>
                <v-icon class="pl-16">close</v-icon>
              </v-btn>
              <v-btn outlined class="ml-2">
                <v-icon>add</v-icon>
              </v-btn>
              <v-btn outlined class="ml-2">
                <v-icon>more_horiz</v-icon>
              </v-btn>

            <v-spacer></v-spacer>
            <v-divider vertical></v-divider>
            <v-autocomplete class="ml-3"
              label="No Environment"
              hide-details
              solo dense>
            </v-autocomplete>
            <v-btn class="ml-3 mr-3"  elevation="1" color="grey darken-3">
              <v-icon>visibility</v-icon>
            </v-btn>
            <v-btn  elevation="1" color="grey darken-3">
              <v-icon>tune</v-icon>
            </v-btn>
          </v-app-bar>
          <div class="mt-10 ml-5">
            <h1 class="mb-4">Good evening!</h1>
            <p class="font-weight-light">Use Launchpad to start something new, pick up where you left off, or explore some resources to help you master Postman.</p>
          </div>
          <v-row>
            <v-col cols="12" lg="6">
              <h3 class="ml-5 mt-10 mb-1">Start something new</h3>
              <v-list style="background:transparent;">

                <v-list-item>
              <v-btn  class="custom-transform-class text-none mr-5 subheading font-weight-bold " >
                <v-icon class="mr-2">subtitles</v-icon>
                <span class="ml-2 font-weight-light">Create a request</span>
              </v-btn>
              </v-list-item>

              <v-list-item>
              <v-btn class="custom-transform-class text-none mr-5 subheading font-weight-bold " >
                <v-icon class="mr-2">text_snippet</v-icon>
                <span class="ml-2 font-weight-light">Create a collection</span>
                <v-icon>arrow_drop_down</v-icon>
              </v-btn>
              </v-list-item>

              <v-list-item>
              <v-btn  class="custom-transform-class text-none mr-5 subheading font-weight-bold " >
                <v-icon class="mr-2">snippet_folder</v-icon>
                <span class="ml-2 font-weight-light">Create an environment</span>
              </v-btn>
              </v-list-item>

              <v-list-item>
              <v-btn text disabled class="custom-transform-class text-none mr-5 subheading font-weight-bold " >
                <v-icon class="mr-2">scatter_plot</v-icon>
                <span class="ml-2 font-weight-light">Create an API</span>
              </v-btn>
              </v-list-item>

              <v-list-item>
              <v-btn  class="custom-transform-class text-none mr-5 subheading font-weight-bold " >
                <v-icon class="mr-2">more_horiz</v-icon>
                <span class="ml-2 font-weight-light">View More</span>
              </v-btn>
              </v-list-item>
              </v-list>

              <h3 class="ml-5 mt-10 ">Recent workspaces</h3>
              <p class="ml-10 mt-8 font-weight-light">Find your most recently used workspaces here</p>

              <h3 class="ml-5 mt-10">Customize</h3>
              <v-switch
                class="ml-5 mb-3"
                v-model="ex11"
                label="Dark mode"
                color="orange darken-3"
                hide-details>
            </v-switch>
            <v-switch
                class="ml-5 mb-3"
                v-model="ex11"
                label="Enable Launchpad"
                color="orange darken-3"
                hide-details>
            </v-switch>
            <v-btn  class="custom-transform-class text-none mr-5 subheading font-weight-bold " >
                <v-icon class="mx-2">more_horiz</v-icon>
                <span class="ml-3 font-weight-light">More settings</span>
              </v-btn>
            </v-col>
            <v-col cols="12" lg="6">

            </v-col>
          </v-row>
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
