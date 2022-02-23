<template>
  <v-app >
    <v-main class="grey lighten-4">
        <Nuxt />
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: 'DefaultLayout',
  data () {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/'
        },
                {
          icon: 'mdi-apps',
          title: 'About',
          to: '/about'
        },
        {
          icon: 'mdi-apps',
          title: 'Text',
          to: '/text'
        },
        {
          icon: 'mdi-apps',
          title: 'Buttons',
          to: '/buttons'
        },
                {
          icon: 'mdi-apps',
          title: 'Home',
          to: '/home'
        },
                {
          icon: 'mdi-apps',
          title: 'Visibility',
          to: '/visibility'
        },
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: "Kenan's New Page"
    }
  }
}
</script>
