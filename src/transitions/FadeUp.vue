<template>
  <transition v-bind="$attrs"
    appear
    enter-active-class="animated fadeInUp"
    leave-active-class="animated fadeOutUp">
    <div v-if="visible">
      <slot/>
    </div>
  </transition>
</template>

<script>
export default {
  name: 'FadeUp',

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
