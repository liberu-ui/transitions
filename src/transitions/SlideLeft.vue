<template>
    <transition appear
        enter-active-class="animated slideInLeft"
        leave-active-class="animated slideOutLeft"
        v-bind="$attrs"
        v-on="$listeners">
        <slot/>
    </transition>
</template>
