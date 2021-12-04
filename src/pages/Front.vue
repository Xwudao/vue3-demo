<script lang="ts" setup="setup">
  import VModel from '@/components/front/VModel.vue';
  import { ref } from 'vue';
  const v = ref('ok');
  const a = ref(18);
</script>

<template>
  <div>
    <VModel v-model="v" v-model:age="a" />
  </div>
</template>

<style lang="scss" scoped></style>
