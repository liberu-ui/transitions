<template>
  <transition v-bind="$attrs"
    appear
    enter-active-class="animate__animated animate__fadeInUp"
    leave-active-class="animate__animated animate__fadeOutUp">
      <slot/>
  </transition>
</template>

<script>
import 'animate.css';

export default {
  name: 'FadeUp',
};
</script>
