<template>
  <transition v-bind="$attrs"
    appear
    enter-active-class="animate__animated animate__slideInLeft"
    leave-active-class="animate__animated animate__slideOutLeft">
      <slot/>
  </transition>
</template>

<script>
import 'animate.css';

export default {
  name: 'SlideLeft',
};
</script>
