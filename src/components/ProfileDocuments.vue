<template>
  <div class="q-mt-xs q-pa-md">
    <div class="section-name">Документы</div>
    <q-btn @click="onClick" no-caps flat class="btn bg-white q-mt-sm q-pa-md">
      <div class="flex justify-between items-center" style="width: 100%">
        <div class="property-name">Удостоверение личности</div>
        <q-icon
          v-if="isClicked"
          name="img:/icons/profile/check-mark.svg"
          class="check-mark"
        />
      </div>
    </q-btn>
    <q-btn @click="onClick" no-caps flat class="btn bg-white q-mt-sm q-pa-md">
      <div class="flex justify-between items-center" style="width: 100%">
        <div class="property-name">СТС (транспорт)</div>
        <q-icon
          v-if="isClicked"
          name="img:/icons/profile/check-mark.svg"
          class="check-mark"
        />
      </div>
    </q-btn>
    <q-btn @click="onClick" no-caps flat class="btn bg-white q-mt-sm q-pa-md">
      <div class="flex justify-between items-center" style="width: 100%">
        <div class="property-name">СТС (прицеп)</div>
        <q-icon
          v-if="isClicked"
          name="img:/icons/profile/check-mark.svg"
          class="check-mark"
        />
      </div>
    </q-btn>
    <q-btn @click="onClick" no-caps flat class="btn bg-white q-mt-sm q-pa-md">
      <div class="flex justify-between items-center" style="width: 100%">
        <div class="property-name">Фото авто</div>
        <q-icon
          v-if="isClicked"
          name="img:/icons/profile/check-mark.svg"
          class="check-mark"
        />
      </div>
    </q-btn>
  </div>
</template>

<script setup lang="ts">
import { ref } from "vue";

const isClicked = ref(false);

const onClick = () => {
  isClicked.value = true;
};
</script>

<style scoped>
.check-mark {
  width: 10px;
  height: 7px;
}
</style>
