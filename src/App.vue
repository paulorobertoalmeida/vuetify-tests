<template>
<!-- App.vue -->

<v-app>
  <v-navigation-drawer app>
    <!-- -->
    hello wolrd
  </v-navigation-drawer>

  <v-app-bar app>
    <!-- -->
    <h1>Hello bar</h1> 
  </v-app-bar>

  <!-- Sizes your content based upon application components -->
  <v-main>

    <!-- Provides the application the proper gutter -->
    <v-container fluid>

      <!-- If using vue-router -->
      <router-view></router-view>
    </v-container>
  </v-main>

  <v-footer app>
    <!-- -->
  </v-footer>
</v-app>
</template>

<script>



export default {
  name: 'App',

  components: {
   
},

  data: () => ({
    //
  }),
};
</script>
