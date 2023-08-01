<template>
  <!-- HELP MODAL -->
  <HelpModal v-model="isHelpButtonClicked" />

  <!-- EDIT PROFILE MODAL -->
  <EditProfileModal v-model="isEditButtonClicked" />


  <div class="q-mt-xs q-pa-md">
    <span class="section-name">Настройки</span>
    <q-btn
      @click="onEditButtonClick"
      no-caps
      flat
      size="md"
      class="btn bg-white q-pa-md q-mt-sm"
    >
      <div class="property-name">Редактировать профиль</div>
    </q-btn>
    <q-btn
      @click="onHelpButtonClick"
      no-caps
      flat
      size="md"
      class="btn bg-white q-pa-md q-mt-sm"
    >
      <div class="property-name">Помощь</div>
    </q-btn>
    <q-btn no-caps flat size="md" class="btn bg-white q-pa-md q-mt-sm"
      ><div class="property-name">Политика конфиденциальности</div>
    </q-btn>
    <q-btn no-caps flat size="md" class="btn bg-white q-pa-md q-mt-sm"
      ><div class="property-name">Правила пользования сервисом</div>
    </q-btn>
  </div>
</template>

<script setup lang="ts">
import { ref } from "vue";
import HelpModal from "./Modals/HelpModal.vue";
import EditProfileModal from "./Modals/EditProfileModal.vue";

const isHelpButtonClicked = ref(false);
const isEditButtonClicked = ref(false);

const onHelpButtonClick = () => {
  isHelpButtonClicked.value = true;
};

const onEditButtonClick = () => {
  isEditButtonClicked.value = true;
}
</script>
