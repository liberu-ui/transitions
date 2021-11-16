<template>
    <transition v-bind="$attrs"
        appear
        enter-active-class="animated fadeInRight"
        leave-active-class="animated fadeOutRight">
        <slot/>
    </transition>
</template>

<script>
export default {
    name: 'FadeRight',
};
</script>
