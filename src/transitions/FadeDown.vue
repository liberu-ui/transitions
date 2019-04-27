<template>
    <transition appear
        enter-active-class="animated fadeInDown"
        leave-active-class="animated fadeOutDown"
        v-bind="$attrs"
        v-on="$listeners">
        <slot/>
    </transition>
</template>

<script>
export default {
    name: 'FadeDown',
};
</script>
