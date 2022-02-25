<script setup>
defineProps({
  camelCase: {
    type: String,
    required: true,
  }  
});
</script>

<template>
  <div>
    {{ camelCase }}
  </div>
</template>
