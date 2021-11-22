<template>
  <transition v-bind="$attrs"
    appear
    enter-active-class="animate__animated animate__fadeInRight"
    leave-active-class="animate__animated animate__fadeOutRight">
      <slot/>
  </transition>
</template>

<script>
import 'animate.css';

export default {
  name: 'FadeRight',
};
</script>
