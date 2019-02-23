<template>
    <transition appear
        enter-active-class="animated slideInUp"
        leave-active-class="animated slideOutUp"
        v-bind="$attrs"
        v-on="$listeners">
        <slot/>
    </transition>
</template>
