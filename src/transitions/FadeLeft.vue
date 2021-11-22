<template>
    <transition v-bind="$attrs"
      appear
      enter-active-class="animate__animated animate__fadeInLeft"
      leave-active-class="animate__animated animate__fadeOutLeft">
        <slot/>
    </transition>
</template>

<script>
import 'animate.css';

export default {
  name: 'FadeLeft',
};
</script>
