<template>
  <div class="home">
     <v-app>
      <v-row>
        <v-col cols="12" lg="3" >
          <div class="px-3" style="border-right:1px solid grey; height: 2050px;">
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
              <v-btn outlined class="ml-2" color="grey">
                <v-icon>add</v-icon>
              </v-btn>
              <v-btn outlined class="ml-2" color="grey">
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
              <v-card outlined class="mt-6 mr-10 pa-3">
                <h3 class="ml-5 mt-5 ">Work smarter with Postman</h3>
                <p class="ml-5 mt-5 font-weight-light">Learn how Postman can help you at every stage of the API development lifecycle with these in-app tutorials.</p>

                <div class="ml-5" >
                  <v-btn class="py-7">
                    <v-icon color="#EF6C00">apartment</v-icon>
                    <span class="ml-4 custom-transform-class text-none font-weight-light">Designing and mocking APIs</span>
                    <span class="custom-transform-class text-none font-weight-light grey--text" style="margin-left:185px">2 lessons</span>
                  </v-btn>
                  <v-btn class="py-7">
                    <v-icon color="#00E676">pest_control</v-icon>
                    <span class="ml-4 custom-transform-class text-none font-weight-light">Debugging and manual testing</span>
                    <span class="custom-transform-class text-none font-weight-light grey--text" style="margin-left:171px">4 lessons</span>
                  </v-btn>
                  <v-btn class="py-7">
                    <v-icon color="#039BE5">integration_instructions</v-icon>
                    <span class="ml-4 custom-transform-class text-none font-weight-light">Automated testing</span>
                    <span class="custom-transform-class text-none font-weight-light grey--text" style="margin-left:260px">4 lessons</span>
                  </v-btn>
                  <v-btn class="py-7"> 
                    <v-icon color="#FFFF00">table_view</v-icon>
                    <span class="ml-4 custom-transform-class text-none font-weight-light">API documentation</span>
                    <span class="custom-transform-class text-none font-weight-light grey--text" style="margin-left:257px">1 lessons</span>
                  </v-btn>
                  <v-btn class="py-7">
                    <v-icon color="#D50000">timeline</v-icon>
                    <span class="ml-4 custom-transform-class text-none font-weight-light">Monotoring</span>
                    <span class="custom-transform-class text-none font-weight-light grey--text" style="margin-left:312px">1 lessons</span>
                  </v-btn>
                  <v-btn class="py-7">
                    <v-icon color="#2E7D32">api</v-icon>
                    <span class="ml-4 custom-transform-class text-none font-weight-light">Collaboration</span>
                    <span class=" custom-transform-class text-none font-weight-light grey--text" style="margin-left:300px">2 lessons</span>
                  </v-btn>
                </div>
              </v-card>

              <v-card outlined class="mt-5 mr-10 pa-3">
                <h3 class="ml-5 mt-5 ">What's new with Postman</h3>
                <h4 class="mt-5 ml-7">It's Rocket Fuel for Your API Skills<span class="ml-3 orange--text text--darken-3 px-1" style="border:1px solid #EF6C00">New</span></h4>
                <p class="ml-7 mt-4 grey--text font-weight-light">Postman Galaxy is the global, virtual API conference whre you can engage with API professionals from all over the world.
                  Attend live demos, ask questions, and connect with fellow attendees to expand your knowledge and network.
                </p>
                <v-btn class="ml-4 orange--text text--darken-3 custom-transform-class text-none"> Register now</v-btn>
                <v-divider class="mx-5 mt-2"></v-divider>
                <h4 class="mt-5 ml-7">The $100,000 Hackathon: Join the Postman API Hack <span class="ml-3 orange--text text--darken-3 px-1" style="border:1px solid #EF6C00">New</span></h4>
                <p class="ml-7 mt-4 grey--text font-weight-light">$100,000 in prizes is up for grabs, Join the Postman API Hack, our first-ever global,
                  virtual hackathon, and submit your brilliant idea(s) for your chance to win.
                </p>
                <v-btn class="ml-4 orange--text text--darken-3 custom-transform-class text-none"> Join the hack</v-btn>
                <v-divider class="mx-5 mt-2"></v-divider>
              </v-card>

              <v-card outlined class="mt-5 mr-10 pa-3">
                <h3 class="ml-5 mt-5 ">Join a team from your org</h3>
                <p class="ml-5 mt-4 font-weight-light">You're not a part of a team. Create a new one to start collaborating.
                </p>
                <v-btn class="ml-2 orange--text text--darken-3 custom-transform-class text-none"> Invite people to collaborate with you</v-btn>
              </v-card>
              
              <v-card outlined class="my-5 mr-10 pa-3">
                <h3 class="ml-5 mt-5 ">Discover</h3>
                <p class="ml-5 mt-4 font-weight-light">Explore some templates and public APIs you might find useful.
                </p>
                <div class="text-center mt-3">
              <v-btn tile class="px-16 custom-transform-class text-none" style="border-bottom: 4px solid #EF6C00">
                Templates 
              </v-btn>
              <v-btn tile class="px-16 custom-transform-class text-none">
                APIs 
              </v-btn>
              <v-divider></v-divider>
                </div>
                 <h4 class="ml-5 mt-5 ">Intro to writing tests - with examples</h4>
                <p class="ml-5 mt-2 grey--text font-weight-light">This collection contains examples of tests that you can use to automate your
                   testing process. Includes basic test syntax, examples of API tests, and integration tests.
                </p>
                <v-divider></v-divider>
                <h4 class="ml-5 mt-5 ">COVID19 API</h4>
                <p class="ml-5 mt-2 grey--text font-weight-light">Corona Virus stats REST API documentation
                </p>
                <v-divider></v-divider>
                <h4 class="ml-5 mt-5 ">Working with GraphQL </h4>
                <p class="ml-5 mt-2 grey--text font-weight-light">CExamples of working with GraphQL endpoints such as using a JSON request body, content-type, and importing queries.
                </p>
                <v-divider></v-divider>
                <div class="text-center">
                  <v-btn class="mt-2 text-capitalize grey--text text--lighten-2">Browse More</v-btn>
                </div>
                </v-card>
            </v-col>
          </v-row>
        </v-col>
      </v-row>
    </v-app>
  </div>
</template>

<script>
export default {
	data: () => ({
		ex11: false,
	}),
};
</script>
