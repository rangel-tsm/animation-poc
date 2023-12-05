<template>
  <q-layout view="hHh lpR fFf">
    <q-header bordered class="bg-transparent text-black" style="height:75px">
      <q-toolbar class="fit">
        <q-toolbar-title>
          <img :src="headerLogo" alt="SMK Logo" style="width: 50%; height: 50px">
        </q-toolbar-title>
        <q-btn v-if="drawerEnabled" flat round icon="menu" @click="leftDrawerOpen = !leftDrawerOpen" />
      </q-toolbar>
    </q-header>

    <q-drawer v-if="drawerEnabled" v-model="leftDrawerOpen" side="left" bordered show-if-above>
      <q-scroll-area class="fit">
        <q-list bordered separator>
          <template v-for="(menuItem, index) in sidebar" :key="index">
            <q-item v-ripple>
              <q-item-section>
                {{ menuItem }}
              </q-item-section>
            </q-item>
          </template>
        </q-list>
      </q-scroll-area>
    </q-drawer>

    <q-page-container>
      <router-view />
    </q-page-container>

    <q-footer elevated class="bg-transparent text-black" style="height:75px">
      <q-toolbar class="fit">
        <q-toolbar-title>
          <img :src="headerLogo" alt="SMK Logo" style="width: 25%; height: 50px">
        </q-toolbar-title>
      </q-toolbar>
    </q-footer>
  </q-layout>
</template>

<script setup>
import { ref } from 'vue'

const drawerEnabled = process.env.DRAWER_ENABLED === 'true'
const headerLogo = process.env.HEADER_LOGO
const leftDrawerOpen = ref(false)
const sidebar = process.env.SIDEBAR_MENU.split(", ")

</script>
