<template>
    <transition appear
        enter-active-class="animated fadeInLeft"
        leave-active-class="animated fadeOutLeft"
        v-bind="$attrs"
        v-on="$listeners">
        <slot/>
    </transition>
</template>
