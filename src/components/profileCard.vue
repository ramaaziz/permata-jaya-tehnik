<template>
  <v-card
    rounded="3xl"
    :height="$vuetify.display.mdAndUp ? 250 : 150"
    class="mt-16 d-flex align-center max-w-full mx-auto shadow-2xl"
  >
    <v-row>
      <v-col>
        <v-img
          src="@/assets/team1.jpg"
          alt="Profile Image"
          height="200"
          contain
        ></v-img>
      </v-col>
      <v-col>
        <v-card-title>John Doe</v-card-title>
        <v-card-subtitle>Software Engineer</v-card-subtitle>
        <v-card-text>
          John is a highly skilled software engineer with over 10 years of
          experience in the industry. He has a strong background in web
          development and is proficient in multiple programming languages.
        </v-card-text>
      </v-col>
    </v-row>
  </v-card>
</template>

<script setup></script>
