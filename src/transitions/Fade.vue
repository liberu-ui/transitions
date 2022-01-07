<template>
  <mirror
    effect="fade">
    <template #default>
      <slot/>
    </template>
  </mirror>
</template>

<script>
import Mirror from './Mirror.vue';

export default {
  name: 'Fade',

  components: { Mirror },
}

</script>
