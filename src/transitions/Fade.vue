<template>
    <transition appear
        enter-active-class="animated fadeIn"
        leave-active-class="animated fadeOut"
        v-bind="$attrs"
        v-on="$listeners">
        <slot/>
    </transition>
</template>
