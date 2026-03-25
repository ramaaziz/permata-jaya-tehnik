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
      max-width="400"
    >
      <v-card
        rounded="xl"
        class="pa-4"
      >
        <v-card-title class="d-flex justify-space-between align-center pl-13">
          {{ title }}
          <v-btn
            icon="mdi-close"
            variant="text"
            @click="dialog = false"
          ></v-btn>
        </v-card-title>

        <CustomCaraousel
          :images="projectImages"
          :desktop-height="600"
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

<style scoped>
/* Forces the image wrapper to use flex centering */
:deep(.v-img__placeholder),
:deep(.v-img__img) {
  display: flex !important;
  align-items: center !important;
  justify-content: center !important;
  /* This ensures the image doesn't just sit at the top of its container */
  position: relative !important;
  margin: auto !important;
}

/* Optional: Add a subtle background color so the empty 
   space around landscape images looks intentional */
:deep(.v-carousel__controls) {
  background: rgba(0, 0, 0, 0.2);
}
</style>
