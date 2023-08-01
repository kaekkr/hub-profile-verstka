<template>
  <q-dialog position="top">
    <q-card
      class="modals flex justify-center"
      style="margin: 15px 10px"
    >
      <!-- EXIT MODAL -->
      <q-card-actions class="exit-modal">
        <q-btn flat icon="img:/icons/profile/exit-modal.svg" v-close-popup />
      </q-card-actions>

      <!-- TITLE -->
      <q-card-section>
        <div class="text-h6">Выйти из аккаунта?</div>
      </q-card-section>

      <!-- TWO BUTTONS -->
      <q-card-actions class="flex q-mb-sm">
        <q-btn
          flat
          no-caps
          class="white-box-2"
          style="background-color: #ecedee"
          v-close-popup
          ><div class="q-px-lg q-py-md" style="font-size: 18px">Отмена</div></q-btn
        >
        <q-btn flat no-caps class="white-box-2 bg-primary text-white"
          ><div class="q-px-lg q-py-md" style="font-size: 18px">Выйти</div></q-btn
        >
      </q-card-actions>
    </q-card>
  </q-dialog>
</template>

<script setup lang="ts"></script>
