<template>
  <!-- EXIT FROM ACCOUNT MODAL  -->
  <ExitAccModal v-model="isExitButtonClicked" />

  <!-- USER INFO -->
  <div class="white-box bg-white">
    <div class="q-pa-md">
      <div class="flex justify-between q-mb-sm">
        <div class="text-h5 text-weight-bold title">Ivanov Ivan Ivanovich</div>
        <q-btn
          @click="exitFromAcc"
          flat
          icon="img:icons/profile/exit-button.svg"
          size="14px"
        />
      </div>
      <div class="section-name" style="color: black">+77777777777</div>
    </div>
  </div>

  <!-- TRANSPORT TYPE -->
  <div class="q-mt-xs q-pa-md">
    <div class="section-name">Тип транспорта</div>
    <div class="white-box-2 bg-white q-pa-md flex items-center q-mt-sm">
      <div class="property-name">Рефрижератор</div>
    </div>
  </div>

  <!-- DOCUMENTS -->
  <ProfileDocuments />

  <!-- BANK CARD -->
  <ProfileBankCard />

  <!-- SETTINGS -->
  <ProfileSettings />

  <!-- PAYMENT ICONS -->
  <div class="q-mb-md flex justify-center">
    <q-icon name="img:/icons/profile/visa.svg" class="q-mr-sm" size="md" />
    <q-icon
      name="img:/icons/profile/mastercard.svg"
      class="q-mr-sm"
      size="md"
    />
    <q-icon name="img:/icons/profile/freedom.svg" class="q-mr-sm" size="md" />
  </div>
</template>

<script setup lang="ts">
import ProfileDocuments from "components/ProfileDocuments.vue";
import ProfileBankCard from "components/ProfileBankCard.vue";
import ProfileSettings from "components/ProfileSettings.vue";
import ExitAccModal from "components/Modals/ExitAccModal.vue";
import { ref } from "vue";

const isExitButtonClicked = ref(false);

const exitFromAcc = () => {
  console.log("qwe");
  isExitButtonClicked.value = true;
};
</script>

<style>
.white-box {
  border-bottom-left-radius: 16px;
  border-bottom-right-radius: 16px;
}

.title {
  width: 50%;
  line-height: normal;
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
  font-size: 16px;
}

.property-name {
  font-size: 15px;
}

.exit-modal {
  position: absolute;
  top: 0px;
  right: -17px;
}

.modals {
  position: relative;
  border-radius: 16px;
}
</style>
