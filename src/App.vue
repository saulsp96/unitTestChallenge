<template>
  <!-- App.vue -->

  <v-app>
    <!--
    <v-navigation-drawer app>
      
    </v-navigation-drawer>
            -->
    <!--
    <v-app-bar app>
      <v-banner>Unit Test Chellenge</v-banner>
    </v-app-bar>
    -->

    <!-- Sizes your content based upon application components -->
    <v-main>
      <v-col>
        <!-- Provides the application the proper gutter -->
        <Form
      /></v-col>
      <v-col> </v-col>
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
import Form from "../src/components/Form";
export default {
  name: "App",

  components: {
    Form,
  },

  data: () => ({
    //
  }),
};
</script>
