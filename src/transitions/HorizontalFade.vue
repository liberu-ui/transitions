<template>
  <transition v-bind="$attrs"
    appear
    :enter-active-class="`animated ${rtl ? 'fadeInRight' : 'fadeInLeft'}`"
    :leave-active-class="`animated ${rtl ? 'fadeOutRight' : 'fadeOutLeft'}`">
    <div v-if="visible">
      <slot/>
    </div>
  </transition>
</template>

<script>
export default {
  name: 'HorizontalFade',

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
