<script setup>
import SlotTest from './components/SlotTest.vue'
import ComponentTest from './components/ComponentTest.vue';
</script>

<template>
  <main>
    <SlotTest v-slot="scope">
      {{ scope.camelCase }}
      {{ scope.withValue }}
      {{ scope.withBind }}
      {{ scope.withVariableBind }}
      {{ scope['fooBar-BAZ_QuX'] }}
    </SlotTest>

    <ComponentTest camelCase="this gives a warning as expected ✔️" />
  </main>
</template>
