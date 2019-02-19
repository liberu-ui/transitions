<template>
    <transition appear
        enter-active-class="zoomIn"
        leave-active-class="zoomOut"
        v-bind="$attrs"
        v-on="$listeners">
        <slot/>
    </transition>
</template>
