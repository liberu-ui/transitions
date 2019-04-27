<template>
    <transition appear
        enter-active-class="animated slideInRight"
        leave-active-class="animated slideOutRight"
        v-bind="$attrs"
        v-on="$listeners">
        <slot/>
    </transition>
</template>

<script>
export default {
    name: 'SlideRight',
};
</script>
