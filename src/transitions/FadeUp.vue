<template>
    <transition v-bind="$attrs"
        appear
        enter-active-class="animated fadeInUp"
        leave-active-class="animated fadeOutUp"
        v-on="$listeners">
        <slot/>
    </transition>
</template>

<script>
export default {
    name: 'FadeUp',
};
</script>
