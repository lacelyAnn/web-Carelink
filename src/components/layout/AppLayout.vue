<script setup></script>

<template>
  <v-responsive>
    <v-app :theme="theme">
      <v-app-bar class="px-3" color="green-lighten-1">
        <v-spacer></v-spacer>
      </v-app-bar>
      <v-main>
        <v-container>
          <slot name="content"></slot>
        </v-container>
      </v-main>

      <v-footer border app color="green-darken-4">
        2024 CareLink University Booking Appointment</v-footer
      >
    </v-app>
  </v-responsive>
</template>
