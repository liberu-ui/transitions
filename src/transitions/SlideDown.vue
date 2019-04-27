<template>
    <transition appear
        enter-active-class="animated slideInDown"
        leave-active-class="animated slideOutUp"
        v-bind="$attrs"
        v-on="$listeners">
        <slot/>
    </transition>
</template>

<script>
export default {
    name: 'SlideDown',
};
</script>
