<template>
  <div class="white-box bg-white">
    <div class="q-pa-md">
      <div class="flex justify-between">
        <div class="text-weight-bold">Ivanov Ivan Ivanovich</div>
        <q-btn flat icon="img:icons/profile/exit-button.svg" size="14px" />
      </div>
      <div>+77777777777</div>
    </div>
  </div>
  <div class="q-mt-xs q-pa-md">
    <div class="section-name">Тип транспорта</div>
    <div class="white-box-2 bg-white q-pa-sm flex items-center">
      <div>Рефрижератор</div>
    </div>
  </div>
  <div class="q-mt-xs q-pa-md">
    <div class="section-name">Документы</div>
    <div class="white-box-2 bg-white q-pa-sm flex items-center">
      <div>Удостоверение личности</div>
    </div>
    <div class="white-box-2 bg-white q-pa-sm flex items-center q-mt-sm">
      <div>СТС (транспорт)</div>
    </div>
    <div class="white-box-2 bg-white q-pa-sm flex items-center q-mt-sm">
      <div>СТС (прицеп)</div>
    </div>
    <div class="white-box-2 bg-white q-pa-sm flex items-center q-mt-sm">
      <div>Фото авто</div>
    </div>
  </div>
  <div class="q-mt-xs q-pa-md">
    <div class="section-name">Банковская карта</div>
    <div class="white-box-2 bg-white q-pa-sm flex items-center">
      <q-icon name="img:/icons/profile/mastercard.svg" class="q-mr-sm"></q-icon>
      <div>•• 7302 07/28</div>
    </div>
  </div>
  <div class="q-mt-xs q-pa-md">
    <div class="section-name">Настройки</div>
    <q-btn
      flat
      size="md"
      class="btn bg-white q-pa-sm q-mt-sm"
    >
    Редактировать профиль
    </q-btn>
    <q-btn
      flat
      size="md"
      class="btn bg-white q-pa-sm q-mt-sm"
    >
      Помощь
    </q-btn>
    <q-btn
      flat
      size="md"
      class="btn bg-white q-pa-sm q-mt-sm"
    >
    Политика конфиденциальности
    </q-btn>
    <q-btn
      flat
      size="md"
      class="btn bg-white q-pa-sm q-mt-sm"
    >
    Правила пользования сервисом
    </q-btn>
  </div>
</template>

<script setup lang="ts"></script>

<style>
.white-box {
  border-bottom-left-radius: 16px;
  border-bottom-right-radius: 16px;
}

.white-box-2 {
  border-radius: 16px;
}

.btn {
  border-radius: 16px;
  width: 100%;
}

.section-name {
  color: #aeafb5;
}
</style>
