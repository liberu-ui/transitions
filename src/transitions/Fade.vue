<template>
    <transition appear
        enter-active-class="fadeIn"
        leave-active-class="fadeOut"
        v-on="$listeners">
        <slot/>
    </transition>
</template>
