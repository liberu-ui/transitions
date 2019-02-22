<template>
    <transition appear
        enter-active-class="animated fadeInRight"
        leave-active-class="animated fadeOutRight"
        v-bind="$attrs"
        v-on="$listeners">
        <slot/>
    </transition>
</template>
