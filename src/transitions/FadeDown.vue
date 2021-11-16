<template>
    <transition v-bind="$attrs"
        appear
        enter-active-class="animated fadeInDown"
        leave-active-class="animated fadeOutDown">
        <slot/>
    </transition>
</template>

<script>
export default {
    name: 'FadeDown',
};
</script>
