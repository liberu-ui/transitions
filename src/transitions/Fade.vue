<template>
    <transition appear
        :mode="mode"
        enter-active-class="fadeIn"
        leave-active-class="fadeOut"
        v-on="$listeners">
        <slot/>
    </transition>
</template>

<script>
export default {
    props: {
        mode: {
            default: null,
        },
    },
}
</script>
