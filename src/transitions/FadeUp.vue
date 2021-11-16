<template>
    <transition v-bind="$attrs"
        appear
        enter-active-class="animated fadeInUp"
        leave-active-class="animated fadeOutUp">
        <slot/>
    </transition>
</template>

<script>
export default {
    name: 'FadeUp',
};
</script>
