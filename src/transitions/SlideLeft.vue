<template>
    <transition v-bind="$attrs"
        appear
        enter-active-class="animated slideInLeft"
        leave-active-class="animated slideOutLeft"
        v-on="$listeners">
        <slot/>
    </transition>
</template>

<script>
export default {
    name: 'SlideLeft',
};
</script>
