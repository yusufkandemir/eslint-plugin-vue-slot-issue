<template>
  <!-- eslint-disable vue/max-attributes-per-line -->
  <div style="color: red">
    <!-- These doesn't give any warnings -->
    <slot
      camelCase
      withValue="foo"
      :withBind="1"
      :withVariableBind="x"
      fooBar-BAZ_QuX
    />
  </div>
</template>

<script setup>
import { ref } from "vue";

const x = ref(99);
</script>
