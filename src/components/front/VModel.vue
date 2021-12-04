<script lang="ts" setup="setup">
  const props = defineProps<{
    modelValue: string;
    age: number;
  }>();
  const emit = defineEmits(['update:age', 'update:modelValue']);
  const handleValue = () => {
    emit('update:modelValue', 'any.....');
  };
  const handleAge = () => {
    emit('update:age', 33);
  };
</script>

<template>
  <div class="div">value: {{ props.modelValue }}</div>
  <div><button class="border border-gray-200" @click="handleValue">change value</button></div>
  <hr />
  <div>age: {{ props.age }}</div>
  <div>
    <button @click="handleAge">Change Age</button>
  </div>
</template>

<style lang="scss" scoped></style>
