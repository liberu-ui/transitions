<template>
    <transition v-bind="$attrs"
        appear
        enter-active-class="animated fadeInLeft"
        leave-active-class="animated fadeOutLeft">
        <slot/>
    </transition>
</template>

<script>
export default {
    name: 'FadeLeft',
};
</script>
