<template>
  <transition v-bind="$attrs"
    appear
    :enter-active-class="`animate__animated animate__${rtl ? 'fadeInRight' : 'fadeInLeft'}`"
    :leave-active-class="`animate__animated animate__${rtl ? 'fadeOutRight' : 'fadeOutLeft'}`">
      <slot/>
  </transition>
</template>

<script>
import 'animate.css';

export default {
  name: 'HorizontalFade',

  props: {
      rtl: {
          type: Boolean,
          default: false,
      },
  },
};
</script>
