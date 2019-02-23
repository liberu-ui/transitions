<template>
    <transition appear
        enter-active-class="animated slideInDown"
        leave-active-class="animated slideOutDown"
        v-bind="$attrs"
        v-on="$listeners">
        <slot/>
    </transition>
</template>
