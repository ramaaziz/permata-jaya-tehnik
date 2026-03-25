<template>
  <v-card
    border
    class="pa-6 text-center fill-height"
    flat
    height="250"
    hover
    rounded="xl"
    @click="dialog = true"
  >
    <v-avatar
      class="mb-4 mt-2"
      :color="iconColor"
      size="80"
    >
      <v-icon
        color="white"
        size="40"
        >{{ icon }}</v-icon
      >
    </v-avatar>

    <v-card-title class="text-h5 font-weight-bold justify-center">
      {{ title }}
    </v-card-title>

    <v-card-subtitle class="mt-2 text-wrap">
      {{ subtitle }}
    </v-card-subtitle>

    <v-card-text class="text-body-2 px-2 pb-2">
      {{ description }}
    </v-card-text>

    <v-dialog
      v-model="dialog"
      max-width="900"
    >
      <v-card
        rounded="xl"
        class="pa-4"
      >
        <v-card-title class="d-flex justify-space-between align-center">
          {{ title }} Documentation
          <v-btn
            icon="mdi-close"
            variant="text"
            @click="dialog = false"
          ></v-btn>
        </v-card-title>

        <CustomCaraousel
          :images="projectImages"
          :desktop-height="550"
          :mobile-height="300"
        />
      </v-card>
    </v-dialog>
  </v-card>
</template>

<script setup>
import { ref } from "vue";
import CustomCaraousel from "./carousel.vue";

defineProps({
  title: String,
  subtitle: String,
  description: String,
  icon: { type: String, default: "mdi-folder-outline" },
  iconColor: { type: String, default: "blue-darken-4" },
  projectImages: Array, // Pass the array of images here
});

const dialog = ref(false);
</script>
