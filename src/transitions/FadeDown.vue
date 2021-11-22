<template>
    <transition v-bind="$attrs"
      appear
      enter-active-class="animate__animated animate__fadeInDown"
      leave-active-class="animate__animated animate__fadeOutDown">
        <slot/>
    </transition>
</template>

<script>
import 'animate.css';

export default {
    name: 'FadeDown',
};
</script>
