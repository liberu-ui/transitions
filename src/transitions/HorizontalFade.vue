<template>
    <transition v-bind="$attrs"
        appear
        :enter-active-class="`animated ${rtl ? 'fadeInRight' : 'fadeInLeft'}`"
        :leave-active-class="`animated ${rtl ? 'fadeOutRight' : 'fadeOutLeft'}`"
        v-on="$listeners">
        <slot/>
    </transition>
</template>

<script>
export default {
    name: 'HorizontalFade',

    props:{
        rtl:{
            type: Boolean,
            default : false,
        }
    }
}
</script>
