<template>
  <q-page class="q-pa-md">
    <q-form @submit="onSubmit" class="q-gutter-md">
      <q-input filled v-model="name" label="Your name" />
      <q-input filled type="email" v-model="email" label="Email" />
      <q-btn label="Submit" type="submit" color="primary" />
    </q-form>
  </q-page>
</template>

<script setup>
import { ref } from 'vue'

const name = ref('')
const email = ref('')

function onSubmit() {
  alert(`Name: ${name.value}\nEmail: ${email.value}`)
}
</script>
