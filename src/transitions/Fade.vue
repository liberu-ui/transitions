<template>
    <transition v-bind="$attrs"
        appear
        enter-active-class="animated fadeIn"
        leave-active-class="animated fadeOut"
        v-on="$listeners">
        <slot/>
    </transition>
</template>

<script>
export default {
    name: 'Fade',
};
</script>
