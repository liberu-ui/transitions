<template>
    <transition v-bind="$attrs"
        appear
        enter-active-class="animated slideInDown"
        leave-active-class="animated slideOutUp"
        v-on="$listeners">
        <slot/>
    </transition>
</template>

<script>
export default {
    name: 'SlideDown',
};
</script>
