<template>
  <v-app>

        <Nuxt />


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
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: "Kenan's New Page"
    }
  }
}
</script>
