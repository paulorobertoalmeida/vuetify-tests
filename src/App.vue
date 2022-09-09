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
        <v-card elevation="24" max-width="444" class="mx-auto">
          <v-system-bar lights-out></v-system-bar>
          <v-carousel
            :continuous="false"
            :cycle="cycle"
            :show-arrows="false"
            hide-delimiter-background
            delimiter-icon="mdi-minus"
            height="300"
          >
            <v-carousel-item v-for="(slide, i) in slides" :key="i">
              <v-sheet :color="colors[i]" height="100%" tile>
                <v-row class="fill-height" align="center" justify="center">
                  <div class="text-h2">{{ slide }} Slide</div>
                </v-row>
              </v-sheet>
            </v-carousel-item>
          </v-carousel>
          <v-list two-line>
            <v-list-item>
              <v-list-item-avatar>
                <v-img src="https://cdn.vuetifyjs.com/images/john.png"></v-img>
              </v-list-item-avatar>
              <v-list-item-content>
                <v-list-item-title>John Leider</v-list-item-title>
                <v-list-item-subtitle>Author</v-list-item-subtitle>
              </v-list-item-content>
              <v-list-item-action>
                <v-switch v-model="cycle" label="Cycle Slides" inset></v-switch>
              </v-list-item-action>
            </v-list-item>
          </v-list>
        </v-card>
        <v-alert icon="$mdiAccount" type="success">hello moto</v-alert>
        <v-avatar color="accent" size="56">P</v-avatar>
        <v-card elevation="2" loading outlined tile>
          <v-card-title>My Text</v-card-title>
          <v-card-subtitle>Subtext</v-card-subtitle>
          <v-card-text>something</v-card-text>
          <v-card-actions>option 1</v-card-actions>
        </v-card>
        <v-chip close-icon="mdi-delete" color="orange">Something We can do</v-chip>
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
  name: "App",

  components: {},

  data: () => ({
    //
  }),
};
</script>
<style>


</style>
