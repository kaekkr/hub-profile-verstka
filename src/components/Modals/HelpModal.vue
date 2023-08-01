<template>
  <q-dialog>
    <q-card
      class="white-box-2 flex justify-center"
      style="position: relative; border-radius: 16px; "
    >
      <q-card-actions class="exit-modal">
        <q-btn flat icon="img:/icons/profile/exit-modal.svg" v-close-popup />
      </q-card-actions>

      <q-card-section>
        <div class="text-h6">Нужна помощь?</div>
      </q-card-section>

      <q-card-section class="q-pt-none text-center" style="width: 100%">
        <div class="property-name" style="color: #aeafb5">
          Пишите в мессенджерах:
        </div>
        <div class="white-box-2 bg-almostwhite q-py-md">
          <q-btn flat icon="img:/icons/profile/telegram.svg" size="xl" />
          <q-btn flat icon="img:/icons/profile/whatsapp.svg" size="xl" />
          <q-btn flat icon="img:/icons/profile/viber.svg" size="xl" />
        </div>
      </q-card-section>

      <q-card-section class="q-pt-none text-center" style="width: 100%">
        <div class="property-name" style="color: #aeafb5">
          Звоните по телефону:
        </div>
        <div class="white-box-2 bg-almostwhite">
          <div class="phone-number text-weight-bold q-pa-xs">
            +7 (777) 777 77-77
          </div>
        </div>
      </q-card-section>

      <q-card-section class="q-pt-none text-center">
        <div class="property-name time-text" style="color: #aeafb5">
          Мы работаем ежедневно с <span class="text-bold">9:00</span> до
          <span class="text-bold">20:00</span>
        </div>
      </q-card-section>
    </q-card>
  </q-dialog>
</template>

<script setup lang="ts"></script>

<style scoped>
.bg-almostwhite {
  background-color: #fafafa;
}

.phone-number {
  font-size: 28px;
}

.time-text {
  inline-size: 180px;
  overflow-wrap: break-word;
}

.section {
  height: 80px;
}
</style>
