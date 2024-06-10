<template>
  <v-navigation-drawer v-model="drawer">
    <v-sheet class="pa-4" color="grey-lighten-4">
      <v-avatar class="mb-4" color="grey-darken-1" size="64"></v-avatar>

      <div>john@google.com</div>
    </v-sheet>

    <v-divider></v-divider>

    <v-list>
      <v-list-item
        color="primary"
        prepend-icon="mdi-file-document-outline"
        value="analitik"
        title="Analitik"
        :to="{ name: 'index' }"
      />
      <v-list-item
        color="primary"
        prepend-icon="mdi-account-outline"
        value="pelanggan"
        title="Pelanggan"
        :to="{ name: 'pelanggan' }"
      />
    </v-list>
  </v-navigation-drawer>
</template>

<script setup>
import { ref } from "vue";

const links = [
  ["mdi-inbox-arrow-down", "Inbox"],
  ["mdi-send", "Send"],
];

const drawer = ref(null);
</script>

<style lang="scss" scoped></style>
