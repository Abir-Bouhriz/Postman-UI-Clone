<template>
  <div>
    <v-card outlined class="mt-6 mr-10 pa-3">
      <h3 class="ml-5 mt-5">Work smarter with Postman</h3>
      <p class="ml-5 mt-5 font-weight-light">
        Learn how Postman can help you at every stage of the API development
        lifecycle with these in-app tutorials.
      </p>

      <div class="ml-5">
        <v-btn class="py-7">
          <v-icon color="#EF6C00">apartment</v-icon>
          <span class="ml-4 custom-transform-class text-none font-weight-light"
            >Designing and mocking APIs</span
          >
          <span
            class="custom-transform-class text-none font-weight-light grey--text"
            style="margin-left: 185px"
            >2 lessons</span
          >
        </v-btn>
        <v-btn class="py-7">
          <v-icon color="#00E676">pest_control</v-icon>
          <span class="ml-4 custom-transform-class text-none font-weight-light"
            >Debugging and manual testing</span
          >
          <span
            class="custom-transform-class text-none font-weight-light grey--text"
            style="margin-left: 171px"
            >4 lessons</span
          >
        </v-btn>
        <v-btn class="py-7">
          <v-icon color="#039BE5">integration_instructions</v-icon>
          <span class="ml-4 custom-transform-class text-none font-weight-light"
            >Automated testing</span
          >
          <span
            class="custom-transform-class text-none font-weight-light grey--text"
            style="margin-left: 260px"
            >4 lessons</span
          >
        </v-btn>
        <v-btn class="py-7">
          <v-icon color="#FFFF00">table_view</v-icon>
          <span class="ml-4 custom-transform-class text-none font-weight-light"
            >API documentation</span
          >
          <span
            class="custom-transform-class text-none font-weight-light grey--text"
            style="margin-left: 257px"
            >1 lessons</span
          >
        </v-btn>
        <v-btn class="py-7">
          <v-icon color="#D50000">timeline</v-icon>
          <span class="ml-4 custom-transform-class text-none font-weight-light"
            >Monotoring</span
          >
          <span
            class="custom-transform-class text-none font-weight-light grey--text"
            style="margin-left: 312px"
            >1 lessons</span
          >
        </v-btn>
        <v-btn class="py-7">
          <v-icon color="#2E7D32">api</v-icon>
          <span class="ml-4 custom-transform-class text-none font-weight-light"
            >Collaboration</span
          >
          <span
            class="custom-transform-class text-none font-weight-light grey--text"
            style="margin-left: 300px"
            >2 lessons</span
          >
        </v-btn>
      </div>
    </v-card>

    <v-card outlined class="mt-5 mr-10 pa-3">
      <h3 class="ml-5 mt-5">What's new with Postman</h3>
      <h4 class="mt-5 ml-7">
        It's Rocket Fuel for Your API Skills<span
          class="ml-3 orange--text text--darken-3 px-1"
          style="border: 1px solid #ef6c00"
          >New</span
        >
      </h4>
      <p class="ml-7 mt-4 grey--text font-weight-light">
        Postman Galaxy is the global, virtual API conference whre you can engage
        with API professionals from all over the world. Attend live demos, ask
        questions, and connect with fellow attendees to expand your knowledge
        and network.
      </p>
      <v-btn
        class="ml-4 orange--text text--darken-3 custom-transform-class text-none"
      >
        Register now
      </v-btn>
      <v-divider class="mx-5 mt-2"></v-divider>
      <h4 class="mt-5 ml-7">
        The $100,000 Hackathon: Join the Postman API Hack
        <span
          class="ml-3 orange--text text--darken-3 px-1"
          style="border: 1px solid #ef6c00"
          >New</span
        >
      </h4>
      <p class="ml-7 mt-4 grey--text font-weight-light">
        $100,000 in prizes is up for grabs, Join the Postman API Hack, our
        first-ever global, virtual hackathon, and submit your brilliant idea(s)
        for your chance to win.
      </p>
      <v-btn
        class="ml-4 orange--text text--darken-3 custom-transform-class text-none"
      >
        Join the hack
      </v-btn>
      <v-divider class="mx-5 mt-2"></v-divider>
    </v-card>

    <v-card outlined class="mt-5 mr-10 pa-3">
      <h3 class="ml-5 mt-5">Join a team from your org</h3>
      <p class="ml-5 mt-4 font-weight-light">
        You're not a part of a team. Create a new one to start collaborating.
      </p>
      <v-btn
        class="ml-2 orange--text text--darken-3 custom-transform-class text-none"
      >
        Invite people to collaborate with you</v-btn
      >
    </v-card>

    <v-card outlined class="my-5 mr-10 pa-3">
      <h3 class="ml-5 mt-5">Discover</h3>
      <p class="ml-5 mt-4 font-weight-light">
        Explore some templates and public APIs you might find useful.
      </p>
      <div class="text-center mt-3">
        <v-btn
          tile
          class="px-16 custom-transform-class text-none"
          style="border-bottom: 4px solid #ef6c00"
        >
          Templates
        </v-btn>
        <v-btn tile class="px-16 custom-transform-class text-none">
          APIs
        </v-btn>
        <v-divider></v-divider>
      </div>
      <h4 class="ml-5 mt-5">Intro to writing tests - with examples</h4>
      <p class="ml-5 mt-2 grey--text font-weight-light">
        This collection contains examples of tests that you can use to automate
        your testing process. Includes basic test syntax, examples of API tests,
        and integration tests.
      </p>
      <v-divider></v-divider>
      <h4 class="ml-5 mt-5">COVID19 API</h4>
      <p class="ml-5 mt-2 grey--text font-weight-light">
        Corona Virus stats REST API documentation
      </p>
      <v-divider></v-divider>
      <h4 class="ml-5 mt-5">Working with GraphQL</h4>
      <p class="ml-5 mt-2 grey--text font-weight-light">
        CExamples of working with GraphQL endpoints such as using a JSON request
        body, content-type, and importing queries.
      </p>
      <v-divider></v-divider>
      <div class="text-center">
        <v-btn class="mt-2 text-capitalize grey--text text--lighten-2"
          >Browse More</v-btn
        >
      </div>
    </v-card>
  </div>
</template>