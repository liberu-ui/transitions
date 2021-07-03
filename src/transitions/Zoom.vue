<template>
    <transition v-bind="$attrs"
        appear
        enter-active-class="animated zoomIn"
        leave-active-class="animated zoomOut"
        v-on="$listeners">
        <slot/>
    </transition>
</template>

<script>
export default {
    name: 'Zoom',
};
</script>
