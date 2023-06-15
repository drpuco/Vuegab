<template>
  <v-app>
    <v-toolbar
      dark
      prominent
      image="https://cdn.vuetifyjs.com/images/backgrounds/vbanner.jpg"
    >
      <v-app-bar-nav-icon white></v-app-bar-nav-icon>

      <v-toolbar-title class="text-white">GAB Bildung</v-toolbar-title>

      <v-spacer></v-spacer>

      <v-btn icon>
        <v-icon>mdi-export</v-icon>
      </v-btn>
    </v-toolbar>
    <v-spacer />
    <v-btn flat href="https://github.com/vuetifyjs/vuetify/releases/latest" target="_blank"> 
    <span class="mr-2">Neue Website</span>
    </v-btn>
    <v-content>
      <HelloWorld/>
    </v-content>
    <v-footer class="bg-grey-lighten-1">
    <v-row justify="center" no-gutters>
      <v-btn
        v-for="link in links"
        :key="link"
        color="white"
        variant="text"
        class="mx-2"
        rounded="xl"
      >
        {{ link }}
      </v-btn>
      <v-col class="text-center mt-4" cols="12">
        {{ new Date().getFullYear() }} — <strong>GAB Bildung</strong>
      </v-col>
    </v-row>
  </v-footer>
  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',

  components: {
    HelloWorld,
  },

  data: () => ({
    //
  }),
}
</script>
