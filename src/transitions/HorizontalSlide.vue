<template>
    <transition appear
        :enter-active-class="'animated ' + (isRTL ? 'slideInRight' : 'slideInLeft' )"
        :leave-active-class="'animated ' + (isRTL ? 'slideOutRight' : 'slideOutLeft') "
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