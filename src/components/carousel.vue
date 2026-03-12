<template>
  <v-row class="text-left mx-4 mb-6 mt-4">
    <v-carousel
      :height="computedHeight"
      aspect-ratio="16/9"
      class="rounded-xl mx-auto"
      cycle
      progress="primary"
      show-arrows="hover"
      hide-delimiter-background
    >
      <v-carousel-item
        v-for="(image, index) in images"
        :key="index"
        :src="image"
        cover
        ><template v-slot:placeholder>
          <div class="d-flex align-center justify-center fill-height">
            <v-progress-circular
              color="primary"
              indeterminate
            ></v-progress-circular>
          </div> </template
      ></v-carousel-item>
    </v-carousel>
  </v-row>
</template>

<script setup>
import { computed } from "vue";
import { useDisplay } from "vuetify";

const props = defineProps({
  images: { type: Array, required: true },
  desktopHeight: { type: Number, default: 750 },
  mobileHeight: { type: Number, default: 250 },
});

const { mdAndUp } = useDisplay();
const computedHeight = computed(() => {
  return mdAndUp.value ? props.desktopHeight : props.mobileHeight;
});
</script>
