<template>
    <div class="signup">
        <v-app>
        <p class="text-right orange--text text--darken-3 mt-5 mr-5">Sign in with Single Sign-On (SSO)</p>
       
      
        <v-row align="center" justify="center">
            <v-card class="mt-15 px-10 pb-3 elevation-2" width="500" >
              <div class="text-center">
                <v-avatar size="150" class="justify-center mt-n16">
                    <v-img src="sign-logo.png"></v-img>
                </v-avatar>
                </div>
                <v-row>
                  <v-col>
                    <h2>Sign In</h2>
                  </v-col>
                  <v-col>
                    <p text class="text-right orange--text text--darken-3 mt-2">Create Account <span class="white--text">instead ?</span></p>
                  </v-col>
                </v-row>
                <p class="mt-2">Email or Username</p>
                <v-text-field class="mt-n3" single-line outlined filled color="orange darken-3"></v-text-field>
                <p class="mt-n5">Password</p>
                <v-text-field class="mt-n3" single-line outlined filled color="orange darken-3"></v-text-field>
                <v-row>
                  <v-col>
                    <v-checkbox class="mt-n5" v-model="ex4" label="Keep me signed in" color="orange darken-3" value="orange darken-3" hide-details></v-checkbox>
                  </v-col>
                  <v-col>
                    <p class="text-right orange--text text--darken-3 mt-n4">Forgot Password</p>
                  </v-col>
                </v-row>
                <v-btn block class="orange darken-3 white--text py-6 custom-transform-class text-none"> Sign In </v-btn>
                <p class="text-center mt-5">or</p>
                <v-btn block class="blue white--text py-6 custom-transform-class text-none"> Sign In with Google</v-btn>
                <p class="text-center mt-5">Blocked from signing in? <span class="orange--text text--darken-3">Try on a web browser.</span></p>
            </v-card>
        </v-row>
        <v-row align="center" justify="center">
            <div class="text-center">
              <p class="grey--text mt-n7">Skip signing in and <router-link to="/home">take me straight to the app </router-link></p>
            </div>
            </v-row>
    </v-app>
    </div>
</template>

<script>
export default {
    
}
</script>