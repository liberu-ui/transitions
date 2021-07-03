<template>
    <transition v-bind="$attrs"
        appear
        :enter-active-class="`animated ${rtl ? 'slideInRight' : 'slideInLeft'}`"
        :leave-active-class="`animated ${rtl ? 'slideOutRight' : 'slideOutLeft'}`"
        v-on="$listeners">
        <slot/>
    </transition>
</template>

<script>
export default {
    name: 'HorizontalSlide',

    props:{
        rtl:{
            type: Boolean,
            default : false,
        }
    }
}
</script>
