<template>
    <v-footer padless style="border-top:1px solid grey">
        <v-btn class="grey--text text-capitalize  subheading font-weight-bold ">
            <v-icon class="mr-2">search</v-icon>
            <span>Find and Replace</span>
        </v-btn>
        <v-btn class="grey--text text-capitalize mr-3 subheading font-weight-bold ">
            <v-icon class="mr-2">sticky_note_2</v-icon>
            <span>Console</span>
        </v-btn>

        <v-spacer></v-spacer>

        <v-btn class="grey--text text-capitalize mr-5 subheading font-weight-bold ">
            <v-icon class="mr-4">school</v-icon>
            <span>Bootcamp</span>
        </v-btn>
        
        <v-btn-toggle dense 
          v-model="toggle_exclusive"
          mandatory>
          <v-btn class="text-capitalize px-8">
            <span class=" orange--text text--darken-3">Build</span>
          </v-btn>
          <v-btn class="text-capitalize px-8">
            <span>Browse</span>
          </v-btn>
        </v-btn-toggle>

        <v-btn class="mr-n5" color="orange darken-3">
            <v-icon >menu_book</v-icon>
        </v-btn>
        <v-btn class="mr-n5" color="grey">
            <v-icon>filter_b_and_w</v-icon>
        </v-btn>
        <v-btn class="mr-n5" color="grey">
            <v-icon>keyboard</v-icon>
        </v-btn>
        <v-btn class="mr-n3" color="grey">
            <v-icon >help</v-icon>
        </v-btn>
    </v-footer>
</template>

<script>
  export default {
    data () {
      return {
        toggle_exclusive: undefined,
      }
    },
  }
</script>