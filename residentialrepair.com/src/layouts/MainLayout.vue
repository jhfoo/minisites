<template>
  <q-layout view="lHh LpR lFf">
    <q-header elevated>
      <q-toolbar class="bg-secondary">
        <q-toolbar-title>Residential Repair</q-toolbar-title>

        <div>v{{ $q.version }}</div>
      </q-toolbar>
    </q-header>
    
    <q-page-container>
      <router-view />
    </q-page-container>

    <q-footer class="bg-white text-white">
      <q-tabs v-model="tab" class="text-teal" dense>
        <q-route-tab name="movies" icon="home" label="Home" to="/" />
        <q-route-tab name="mails" icon="mail" label="Services" to="/services" />
        <q-tab name="alarms" icon="alarm" label="Gallery" />
      </q-tabs>
    </q-footer>
  </q-layout>
</template>

<script>
import { defineComponent, ref } from 'vue'
import EssentialLink from 'components/EssentialLink.vue'

export default defineComponent({
  name: 'MainLayout',

  components: {
    EssentialLink
  },

  setup () {
    const leftDrawerOpen = ref(false)

    return {
      essentialLinks: linksList,
      leftDrawerOpen,
      toggleLeftDrawer () {
        leftDrawerOpen.value = !leftDrawerOpen.value
      }
    }
  }
})
</script>
