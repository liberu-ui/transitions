<template>
    <transition appear
        enter-active-class="animated zoomIn"
        leave-active-class="animated zoomOut"
        v-bind="$attrs"
        v-on="$listeners">
        <slot/>
    </transition>
</template>

<script>
export default {
    name: 'Zoom',
};
</script>
