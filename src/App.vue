<template>
  <v-app>
    <v-app-bar
      app
      color="primary"
      dark
      dense
      elevation
    >
      <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
    </v-app-bar>
    <v-divider></v-divider>
    <v-navigation-drawer
        v-model="drawer"
        color="#09151E"
        app
        left
        :mini-variant.sync="mini"
    >
        <v-divider></v-divider>
        <v-list nav dense>
            <v-list-item link href="#">
                <v-list-item-icon>
                    <v-icon color="white" small>mdi-lightbulb</v-icon>
                </v-list-item-icon>
                <v-list-item-title class="title">Blue</v-list-item-title>
            </v-list-item>
        </v-list>
    </v-navigation-drawer>

    <v-main>
      <v-container>
        teste
      </v-container>

      
    </v-main>
    <v-footer>
      kjhkhj
    </v-footer>
  </v-app>
</template>

<script>
// import HelloWorld from './components/HelloWorld';

export default {
  name: 'App',

  components: {
    // HelloWorld,
  },

  data: () => ({
    drawer: true,
    mini: true,
  }),
};
</script>
