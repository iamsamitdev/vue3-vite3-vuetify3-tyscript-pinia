<template>
  <!-- <div class="d-flex align-center flex-column">

    <div class="text-subtitle-2"> 
      <v-icon icon="mdi-home" /> 
      <v-icon icon="mdi-menu" /> 
      <v-icon icon="mdi-dots-vertical" />
      <v-icon icon="mdi-menu-swap" />
      
    With props</div>

    <v-card
      width="400"
      title="This is a title"
      subtitle="This is a subtitle"
      text="This is content"
    ></v-card>

    <div class="mt-4 text-subtitle-2">With slots</div>

    <v-card width="400">
      <template v-slot:title>
        This is a title
      </template>

      <template v-slot:subtitle>
        This is a subtitle
      </template>

      <template v-slot:text>
        This is content
      </template>
    </v-card>

    <div class="mt-4 text-subtitle-2">With markup</div>

    <v-card width="400">
      <v-card-item>
        <v-card-title>This is a title</v-card-title>

        <v-card-subtitle>This is a subtitle</v-card-subtitle>
      </v-card-item>

      <v-card-text>
        This is content
      </v-card-text>
    </v-card>
  </div> -->

  <v-app id="inspire">

    <v-navigation-drawer v-model="drawer">
      <!-- somthing -->
     
    </v-navigation-drawer>

    <v-app-bar color="primary">
      <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>

      <v-toolbar-title>
        Vuetify3
        <v-btn prepend-icon="mdi-vuetify" @click="toggleTheme()">
          Dark
        </v-btn>
      </v-toolbar-title>

      
    </v-app-bar>

    <v-main color="primary">
      <!-- Some Content -->
    </v-main>

  </v-app>

</template>

<script setup lang="ts">

  import { ref } from 'vue';
  const drawer = ref(true)

  const toggleTheme = () => {

  }

  // toggleTheme() {
  //     this.$vuetify.theme.dark = !this.$vuetify.theme.dark;
  // }

</script>

<style scoped>

</style>