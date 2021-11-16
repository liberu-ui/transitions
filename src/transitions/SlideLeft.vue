<template>
    <transition v-bind="$attrs"
        appear
        enter-active-class="animated slideInLeft"
        leave-active-class="animated slideOutLeft">
        <slot/>
    </transition>
</template>

<script>
export default {
    name: 'SlideLeft',
};
</script>
