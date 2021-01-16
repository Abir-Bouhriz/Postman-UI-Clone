<template>
  <v-app>
  <Navbar />
    <v-main class="mx-5 mb-5">
      <router-view></router-view>
    </v-main>
    <Footer />
  </v-app>
</template>

<script>
import Navbar from '@/components/Navbar';
import Footer from '@/components/Footer';
export default {
  name: 'App',
  components: { Navbar , Footer},

  data: () => ({
    //
  }),
};
</script>