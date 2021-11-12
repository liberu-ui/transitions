<template>
    <transition appear
        v-bind="$attrs"
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
