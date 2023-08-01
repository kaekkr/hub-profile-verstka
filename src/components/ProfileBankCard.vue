<template>
  <div class="q-mt-xs q-pa-md">
    <span class="section-name">Банковская карта</span>
    <div class="white-box-2 bg-white q-pa-md q-mt-sm">
      <div v-if="bankCard" class="flex items-center">
        <q-icon name="img:/icons/profile/mastercard.svg" class="q-mr-md bank-card" />
        <div class="property-name">•• 7302 07/28</div>
      </div>
      <div v-else>
        <div class="flex items-center q-mb-sm">
          <q-icon
            name="img:/icons/profile/exclamation-point.svg"
            class="exclamation-point"
          />
          <div class="property-name text-primary q-ml-sm">Карта не указана</div>
        </div>
        <q-btn
          @click="addBankCard"
          no-caps
          flat
          class="btn bg-primary"
          padding="sm"
          style="height: 70px"
          text-color="white"
          ><div class="add-card-title">Добавить карту</div>
        </q-btn>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from "vue";

const bankCard = ref(false);

const addBankCard = () => {
  bankCard.value = true;
};
</script>

<style scoped>
.exclamation-point {
  width: 19px;
  height: 19px;
}

.add-card-title {
  font-size: 18px;
}

.bank-card {
  width: 26px;
  height: 26px;
}
</style>
