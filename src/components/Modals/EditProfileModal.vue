<template>
  <q-dialog>
    <q-card
      class="white-box-2 flex justify-center"
      style="position: relative; border-radius: 16px; background-color: #f6f6f4 "
    >
      <q-card-actions class="exit-modal">
        <q-btn flat icon="img:/icons/profile/exit-modal.svg" v-close-popup />
      </q-card-actions>

      <q-card-section>
        <div class="text-h6">Редактировать профиль</div>
      </q-card-section>

      <q-card-section class="q-pt-none text-center" style="width: 100%">
        <q-btn no-caps flat size="md" class="btn bg-white q-pa-md q-mt-sm"
          ><div class="property-name">Изменить транспорт</div>
        </q-btn>
        <q-btn no-caps flat size="md" class="btn bg-white q-pa-md q-mt-sm"
          ><div class="property-name">Изменить прицеп</div>
        </q-btn>
        <q-btn no-caps flat size="md" class="btn bg-white q-pa-md q-mt-sm"
          ><div class="property-name">Изменить номер телефона</div>
        </q-btn>
        <q-btn no-caps flat size="md" class="btn bg-white q-pa-md q-mt-sm"
          ><div class="property-name">Изменить номер банковской карты</div>
        </q-btn>
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
