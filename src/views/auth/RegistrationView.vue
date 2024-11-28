<script setup>
import AppLayout from '@/components/layout/AppLayout.vue'
</script>

<template>
  <AppLayout>
    <template #content>
      <v-row>
        <v-col cols="8" md="5" class="mx-auto">
          <v-card
            class="mx-auto" color="#DCEFC8"
            elevation="24"
          >

          <v-card-title class="text-center">
            <v-img class="mx-auto" src="/images/logo-favicon.webp" width="20%"></v-img>

              <h1 class="font-weight-black text-center">CareLink</h1>
              <p class="font-weight-black"> <h6>Register Page</h6> </p>

              <v-divider class="my-1"></v-divider>
            </v-card-title>

            <v-card-text class="bg-surface-dark pt-4"
              ><v-form fast-fail @submit.prevent>
                <v-text-field
                  label="Name"
                  prepend-icon="mdi-account"
                  variant="solo-inverted"
                ></v-text-field>

                <v-text-field
                  label="Last"
                  prepend-icon="mdi-account"
                  variant="solo-inverted"
                ></v-text-field>

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

                <v-btn class="mt-2" type="submit" block color="light"  prepend-icon="mdi-login">Register</v-btn>
              </v-form>
              <v-divider class="my-5"></v-divider>
              <h5 class="text-center">
                Already have an account?
                <RouterLink to="login">Click here to Login</RouterLink>
              </h5>
            </v-card-text>
          </v-card>
        </v-col>
      </v-row>
    </template>
  </AppLayout>
</template>
