<template>
  <transition v-bind="$attrs"
    appear
    enter-active-class="animate__animated animate__slideInUp"
    leave-active-class="animate__animated animate__slideOutDown">
      <slot/>
  </transition>
</template>

<script>
import 'animate.css';

export default {
  name: 'SlideUp',
};
</script>
