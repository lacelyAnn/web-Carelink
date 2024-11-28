<script setup>
import AppLayout from '@/components/layout/AppLayout.vue'
</script>

<template>
  <AppLayout>
    <template #content>
      <v-row>
        <v-col cols="12" md="6" class="mx-auto">
          <v-card class="mx-auto" color="#DCEFC8" elevation="24">
            <v-card-title class="text-center">

              <v-img class="mx-auto" src="/images/logo-favicon.webp" width="20%"></v-img>
              <h2 class="font-weight-black text-center">CareLink</h2>
              <p class="font-weight-black"> <h6>Login Page</h6> </p>

              <v-divider class="my-1"></v-divider>
            </v-card-title>

            <v-card-text class="bg-surface-dark pt-4"
              ><v-form fast-fail @submit.prevent>
                <v-text-field
                  label="Email"
                  prepend-icon="mdi-account"
                  variant="solo-inverted"
                ></v-text-field>

                <v-text-field
                  label="Password"
                  type="password"
                  prepend-icon="mdi-lock"
                  variant="solo-inverted"
                ></v-text-field>

                <v-btn class="mt-2" type="submit" block color="light" prepend-icon="mdi-login">Login</v-btn>
              </v-form>

              <v-divider class="my-5"></v-divider>
              <h5 class="text-center">
                Don't have an account?
                <RouterLink to="register">Click here to register</RouterLink>
              </h5>
            </v-card-text>
          </v-card>
        </v-col>
      </v-row>
    </template>
  </AppLayout>
</template>
