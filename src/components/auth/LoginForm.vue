<template>
  <v-form fast-fail @submit.prevent>
    <v-text-field label="Email" prepend-icon="mdi-account" variant="solo-inverted"></v-text-field>

    <v-text-field
      label="Password"
      type="password"
      prepend-icon="mdi-lock"
      variant="solo-inverted"
    ></v-text-field>

    <v-btn class="mt-2" type="submit" block color="light" prepend-icon="mdi-login">Login</v-btn>
  </v-form>
</template>
