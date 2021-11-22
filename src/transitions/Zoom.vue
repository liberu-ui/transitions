<template>
  <transition v-bind="$attrs"
    appear
    enter-active-class="animate__animated animate__zoomIn"
    leave-active-class="animate__animated animate__zoomOut">
      <slot/>
  </transition>
</template>

<script>
import 'animate.css';

export default {
  name: 'Zoom',
};
</script>
