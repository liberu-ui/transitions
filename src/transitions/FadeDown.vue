<template>
    <transition v-bind="$attrs"
      appear
      enter-active-class="animated fadeInDown"
      leave-active-class="animated fadeOutDown">
      <div v-if="visible">
        <slot/>
      </div>
    </transition>
</template>

<script>
export default {
    name: 'FadeDown',

    data: () => ({
      visible: false,
    }),

    mounted() {
      this.visible = true;
    },

    unmounted() {
      this.visible = false;
    }
};
</script>
