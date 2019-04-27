<template>
    <transition appear
        enter-active-class="animated fadeInUp"
        leave-active-class="animated fadeOutUp"
        v-bind="$attrs"
        v-on="$listeners">
        <slot/>
    </transition>
</template>

<script>
export default {
    name: 'FadeUp',
};
</script>
