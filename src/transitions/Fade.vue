<template>
  <transition v-bind="$attrs"
    appear
    mode="in-out"
    enter-active-class="animate__animated animate__fadeIn"
    leave-active-class="animate__animated animate__fadeOut">
      <slot/>
  </transition>
</template>

<script>
import 'animate.css';

export default {
  name: 'Fade',
};
</script>
