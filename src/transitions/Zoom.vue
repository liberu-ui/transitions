<template>
    <transition v-bind="$attrs"
        appear
        enter-active-class="animated zoomIn"
        leave-active-class="animated zoomOut">
        <slot/>
    </transition>
</template>

<script>
export default {
    name: 'Zoom',
};
</script>
