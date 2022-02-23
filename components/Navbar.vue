<template>
  <div class="Navbar">
    <v-app-bar text app>
      <v-app-bar-nav-icon class="red--text" @click="drawer = !drawer"></v-app-bar-nav-icon>
    <v-app-bar-title class="text-uppercase grey-- text text-no-wrap">
      <span class="font-weight-light">Todo</span>
        <span>Ken</span>
    </v-app-bar-title>
        <v-spacer></v-spacer>
      <v-btn text color="grey lighten-3">
      <span>Sign Out</span>
      <v-icon right>mdi-arrow-right-bold-box-outline</v-icon>
      </v-btn>
      </v-app-bar>

      <v-navigation-drawer app v-model="drawer" class="red">
        <v-container>
        <v-list>
          <v-list-tile v-for="link in links" :key="link.text">
            <v-list-tile-action>
              <v-icon class="white--text"> {{ link.icon }}</v-icon>
            </v-list-tile-action>
            <v-list-tile-content>
              <v-list-tile-title class="white--text">
                <NuxtLink class="white--text" style="text-decoration-line: none" :to="link.route">{{ link.text }}</NuxtLink>
              </v-list-tile-title>
                <br/>
                <br/>
            </v-list-tile-content>
          </v-list-tile>
        </v-list>
        </v-container>
      </v-navigation-drawer>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        drawer: false,
        links:
          [
            { icon: 'mdi-view-dashboard', text: 'Dashboard', route: '/dashboard' },
            { icon: 'mdi-folder', text: 'My Projects', route: '/projects'},
            { icon: 'mdi-account', text: 'Team', route: '/team'}
          ]
      }
    }
  }
</script>
