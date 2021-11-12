<template>
    <transition v-bind="$attrs"
        appear
        enter-active-class="animated slideInRight"
        leave-active-class="animated slideOutRight"
        v-on="$listeners">
        <slot/>
    </transition>
</template>

<script>
export default {
    name: 'SlideRight',
};
</script>
