<template>
    <transition v-bind="$attrs"
        appear
        enter-active-class="animated slideInUp"
        leave-active-class="animated slideOutDown"
        v-on="$listeners">
        <slot/>
    </transition>
</template>

<script>
export default {
    name: 'SlideUp',
};
</script>
