<script setup>
import AppLayout from '@/components/layout/AppLayout.vue'
import RegisterForm from '@/components/auth/RegisterForm.vue';
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

            <v-card-text class="bg-surface-dark pt-4">

              <RegisterForm></RegisterForm>

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
