<template>
  <v-app>
    <v-main>
      <div class="h-100 flex-layout">
        <nuxt />
      </div>
    </v-main>
  </v-app>
</template>

<script>
export default {
  data() {
    return {};
  },
};
</script>

<style scoped>
.flex-layout {
  display: flex !important;
  flex-direction: column !important;
  flex-grow: 1 !important;
}
</style>
