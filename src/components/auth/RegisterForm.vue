<template>
  <v-form fast-fail @submit.prevent>
    <v-text-field label="Name" prepend-icon="mdi-account" variant="solo-inverted"></v-text-field>

    <v-text-field label="Last" prepend-icon="mdi-account" variant="solo-inverted"></v-text-field>

    <v-text-field
      label="ID- Number"
      prepend-icon="mdi-card-account-details"
      variant="solo-inverted"
    ></v-text-field>

    <v-text-field
      label="Password"
      type="password"
      prepend-icon="mdi-lock"
      variant="solo-inverted"
    ></v-text-field>

    <v-text-field
      label="Password Confirmation"
      type="password"
      prepend-icon="mdi-lock-open"
      variant="solo-inverted"
    ></v-text-field>

    <v-btn class="mt-2" type="submit" block color="light" prepend-icon="mdi-login">Register</v-btn>
  </v-form>
</template>
