<template>
  <q-layout view="lHh Lpr lFf">
    <q-toolbar class="bg-primary text-white q-my-md shadow-2">
      <q-btn flat round dense icon="menu" class="q-mr-sm" />
      <q-separator dark vertical inset />
      <q-btn stretch flat label="Link" />

      <q-space />

      
      <q-separator dark vertical />
      <q-btn stretch flat label="About" />
      <q-separator dark vertical />
      <q-btn stretch flat label="Blog" />
    </q-toolbar>
    

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script setup>
import { ref } from 'vue'


defineOptions({
  name: 'MainLayout'
})


function toggleLeftDrawer () {
  leftDrawerOpen.value = !leftDrawerOpen.value
}
</script>
