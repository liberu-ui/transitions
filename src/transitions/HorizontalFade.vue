<template>
    <transition appear
        :enter-active-class="'animated ' + (rtl ? 'fadeInRight' : 'fadeInLeft' )"
        :leave-active-class="'animated ' + (rtl ? 'fadeOutRight' : 'fadeOutLeft') "
        v-bind="$attrs"
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