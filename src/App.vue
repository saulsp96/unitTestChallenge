<template>
  <!-- App.vue -->

  <v-app>
    <v-parallax
      height="1000"
      src="https://cdn.vuetifyjs.com/images/parallax/material.jpg"
    >
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
        <div class="left-column">
          <Form />
        </div>
        <div class="right-column"><DataIterator /></div>
        <v-container fluid>
          <!-- If using vue-router -->
          <router-view></router-view>
        </v-container>
      </v-main>

      <v-footer app>
        <!-- -->
      </v-footer>
    </v-parallax>
  </v-app>
</template>

<script>
import Form from "../src/components/Form";
import DataIterator from "../src/components/List";
export default {
  name: "App",

  components: {
    Form,
    DataIterator,
  },

  data: () => ({
    //
  }),
};
</script>
