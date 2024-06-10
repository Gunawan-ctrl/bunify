<template>
  <VApp>
    <LayoutSidebar />
    <LayoutHeader />
    <VMain>
      <VContainer class="py-8 px-6" fluid>
        <slot />
      </VContainer>
    </VMain>
    <LayoutFooter />
  </VApp>
</template>

<script setup>
const links = [
  ["mdi-inbox-arrow-down", "Inbox"],
  ["mdi-send", "Send"],
  ["mdi-delete", "Trash"],
  ["mdi-alert-octagon", "Spam"],
];

const drawer = ref(null);
</script>

<script>
export default {
  data: () => ({
    cards: ["Today", "Yesterday"],
    drawer: null,
    links: [
      ["mdi-inbox-arrow-down", "Inbox"],
      ["mdi-send", "Send"],
      ["mdi-delete", "Trash"],
      ["mdi-alert-octagon", "Spam"],
    ],
  }),
};
</script>

<style></style>
