<template>
  <v-card
    rounded="3xl"
    :height="$vuetify.display.mdAndUp ? 250 : 150"
    class="mt-16 d-flex align-center max-w-full mx-auto shadow-2xl"
  >
    <v-row>
      <v-col>
        <v-img
          src="@/assets/team/team1.jpg"
          alt="Profile Image"
          height="200"
          contain
          class="py-6 px-2 rounded"
        ></v-img>
      </v-col>
      <v-col class="py-4">
        <v-card-title class="py-1">John Doe</v-card-title>
        <v-card-subtitle class="py-1">Software Engineer</v-card-subtitle>
        <v-card-text>
          lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do
          eiusmod tempor incididunt
        </v-card-text>
      </v-col>
    </v-row>
  </v-card>
</template>

<script setup></script>
