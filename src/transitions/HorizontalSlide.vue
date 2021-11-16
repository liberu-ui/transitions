<template>
    <transition v-bind="$attrs"
        appear
        :enter-active-class="`animated ${rtl ? 'slideInRight' : 'slideInLeft'}`"
        :leave-active-class="`animated ${rtl ? 'slideOutRight' : 'slideOutLeft'}`">
        <slot/>
    </transition>
</template>

<script>
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
