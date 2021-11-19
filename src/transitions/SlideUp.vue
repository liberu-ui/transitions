<template>
  <transition v-bind="$attrs"
    appear
    enter-active-class="animated slideInUp"
    leave-active-class="animated slideOutDown">
    <div v-if="visible">
      <slot/>
    </div>
  </transition>
</template>

<script>
export default {
  name: 'SlideUp',

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
