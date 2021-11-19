<template>
  <transition v-bind="$attrs"
    appear
    :enter-active-class="`animated ${rtl ? 'slideInRight' : 'slideInLeft'}`"
    :leave-active-class="`animated ${rtl ? 'slideOutRight' : 'slideOutLeft'}`">
    <div v-if="visible">
      <slot/>
    </div>
  </transition>
</template>

<script>
export default {
  name: 'HorizontalSlide',

  props: {
      rtl: {
          type: Boolean,
          default: false,
      },
  },

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
