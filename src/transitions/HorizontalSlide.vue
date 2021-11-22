<template>
  <transition v-bind="$attrs"
    appear
    :enter-active-class="`animate__animated animate__${rtl ? 'slideInRight' : 'slideInLeft'}`"
    :leave-active-class="`animate__animated animate__${rtl ? 'slideOutRight' : 'slideOutLeft'}`">
      <slot/>
  </transition>
</template>

<script>
import 'animate.css';

export default {
  name: 'HorizontalSlide',

  props: {
      rtl: {
          type: Boolean,
          default: false,
      },
  },
};
</script>
