<template>
    <transition appear
        :enter-active-class="'animated ' + (isRTL ? 'slideInLeft' : 'slideInRight' )"
        :leave-active-class="'animated ' + (isRTL ? 'slideOutLeft' : 'slideOutRight') "
        v-bind="$attrs"
        v-on="$listeners">
        <slot/>
    </transition>
</template>

<script>
export default {
    name: 'HorizontalSlide',

    props:{
        isRTL:{
            type: Boolean,
            default : false,
        }
    }
}
</script>