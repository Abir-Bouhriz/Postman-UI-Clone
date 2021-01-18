<template>
    <v-app-bar app flat height="60">
        <v-btn dense elevation="2" color="orange darken-3" class="text-capitalize mr-3 subheading font-weight-bold " >
            <v-icon class="mr-2 ml-n2">add_box</v-icon>
            <span class="mr-n2">New</span>
        </v-btn>
        <v-btn elevation="1" color="grey darken-3" class="grey--text text-capitalize mr-3 subheading font-weight-bold " >
            Import
        </v-btn>
        <v-btn elevation="1" color="grey darken-3" class="grey--text text-capitalize mr-3 subheading font-weight-bold " >
            Runner
        </v-btn>
        <v-menu offset-y>
      <template v-slot:activator="{ on, attrs }">
        <v-btn
          elevation="1" color="grey darken-3" class="grey--text text-capitalize mr-3 subheading font-weight-bold "
          v-bind="attrs"
          v-on="on">
          <v-icon class="mr-1 ml-n2" color="grey">post_add</v-icon>
        <v-icon class="mr-n2" color="grey">arrow_drop_down</v-icon>
        </v-btn>
      </template>
      <v-list height="160">
          <v-list-item-title class="ml-4 body-2 grey--text">OPEN NEW</v-list-item-title>
          <v-row>
              <v-col>
        <v-list-item dense
          v-for="(item, index) in items"
          :key="index">
          <v-list-item-title class="body-2 mt-n2">{{ item.title }}</v-list-item-title>
        </v-list-item>
        </v-col>
        <v-col>
            <v-list-item dense
          v-for="(link, i) in links"
          :key="i">
          <v-list-item-title class="body-2 mt-n2 grey--text">{{ link.title }}</v-list-item-title>
        </v-list-item>
        </v-col>
        </v-row>
      </v-list>
    </v-menu>

        <v-spacer></v-spacer>

        <v-btn text  class="text-capitalize mr-5 subheading font-weight-bold " >
            <v-icon class="mr-2">dashboard</v-icon>
            <span class="mr-2">My Work Space</span>
            <v-icon>arrow_drop_down</v-icon>
        </v-btn>
        <v-btn elevation="1" color="grey darken-3" class="text-capitalize mr-5 subheading font-weight-bold " >
            <v-icon class="mr-2 ml-n2">person_add_alt_1</v-icon>
            <span class="mr-n2">Invite</span>
        </v-btn>
    
      <v-spacer></v-spacer>
        <v-tooltip bottom>
            <template v-slot:activator="{ on, attrs }">
                <v-btn fab small v-bind="attrs" v-on="on" class="mr-2 orange darken-3" >
                    <v-icon > autorenew </v-icon>
                </v-btn>
            </template>
            <span>Sync your API requests across devices</span>
        </v-tooltip>
        <v-tooltip bottom>
            <template v-slot:activator="{ on, attrs }">
                <v-btn fab small v-bind="attrs" v-on="on" class="mr-2" >
                    <v-icon > wifi_tethering </v-icon>
                </v-btn>
            </template>
            <span>Capture requests ans cookies with Postman</span>
        </v-tooltip>
        <v-tooltip bottom>
            <template v-slot:activator="{ on, attrs }">
                <v-btn fab small v-bind="attrs" v-on="on" class="mr-2" >
                    <v-icon > settings </v-icon>
                </v-btn>
            </template>
            <span>Settings</span>
        </v-tooltip>
        <v-tooltip bottom>
            <template v-slot:activator="{ on, attrs }">
                <v-btn fab small class="mr-2" v-bind="attrs" v-on="on" >
                    <v-icon > notifications</v-icon>
                </v-btn>
            </template>
            <span>Notifications</span>
        </v-tooltip>
        <v-btn fab small class="mr-2" >
            <v-icon > favorite </v-icon>
        </v-btn>
        <v-tooltip bottom>
            <template v-slot:activator="{ on, attrs }">
                <v-btn fab small v-bind="attrs" v-on="on" class="mr-2 teal lighten-2" >
                    <v-icon > account_tree </v-icon>
                </v-btn>
            </template>
            <span>Manage accounts</span>
        </v-tooltip>
        <v-btn elevation="1" color="grey darken-3" class="text-capitalize subheading font-weight-bold " >
            <router-link to="/signup"></router-link>
            <span class="mr-1 grey--text ">Upgrade</span>
            <v-icon class="mr-n2" color="grey">arrow_drop_down</v-icon>
        </v-btn>
    </v-app-bar>
</template>

<script>
export default {
     data: () => ({
      items: [
        { title: 'Tab' },
        { title: 'Postman Window' },
        { title: 'Runner Window' },
      ],
      links: [
        { title: 'Ctrl+T' },
        { title: 'Ctrl+Shift+N' },
        { title: 'Ctrl+Shift+R' },
      ],
    }),
}
</script>