<template>
  <v-app-bar
    app
    elevation="0"
    :height="70"
    class="border"
    shrink-on-scroll
    prominent
  >
    <v-list-item>
      <template v-slot:prepend>
        <v-btn size="medium" variant="text" color="black" />
      </template>
      <template v-slot:title>
        <span class="font-weight-bold text-h6">Analitik</span>
      </template>
    </v-list-item>
    <v-spacer />
    <v-app-bar-nav-icon
      v-if="$vuetify.display.mobile"
      class="text-black"
      @click="$emit('drawerEvent')"
      color="black"
    >
    </v-app-bar-nav-icon>
  </v-app-bar>
</template>

<script setup lang="ts"></script>

<style lang="scss" scoped></style>
