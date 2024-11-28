<script setup>
import AppLayout from '@/components/layout/AppLayout.vue'
import LoginForm from '@/components/auth/LoginForm.vue';
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

            <v-card-text class="bg-surface-dark pt-4">

            <LoginForm></LoginForm>

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
