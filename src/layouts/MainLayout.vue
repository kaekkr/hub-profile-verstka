<template>
  <q-layout view="hhh lpR fFf">
    <q-page-container>
      <router-view />
    </q-page-container>

    <q-footer class="bg-custom text-black">
      <q-toolbar>
        <q-toolbar-title>
          <div class="flex flex-center">TEST</div>
        </q-toolbar-title>
      </q-toolbar>
    </q-footer>
  </q-layout>
</template>

<script setup lang="ts"></script>

<style>
.bg-custom {
  background-color: rgba(16, 18, 28, 0.03);
}
</style>
