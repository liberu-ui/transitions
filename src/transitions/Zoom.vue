<template>
  <transition v-bind="$attrs"
    appear
    enter-active-class="animated zoomIn"
    leave-active-class="animated zoomOut">
    <div v-if="visible">
      <slot/>
    </div>
  </transition>
</template>

<script>
export default {
  name: 'Zoom',

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
