<template>
  <transition v-bind="$attrs"
    appear
    enter-active-class="animate__animated animate__slideInRight"
    leave-active-class="animate__animated animate__slideOutRight">
      <slot/>
  </transition>
</template>

<script>
import 'animate.css';

export default {
  name: 'SlideRight',
};
</script>
