<script setup lang="ts">
import { inject } from 'vue';

import { useScrollLock } from '@ittlr-core/composables';

useScrollLock();
const id = inject('DISMISSABLE_MODAL_ID');
</script>
<template>
  <div :data-dismissable-modal="id" class="bg-overlay inset-0"></div>
</template>
