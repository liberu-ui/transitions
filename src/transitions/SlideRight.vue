<template>
  <transition v-bind="$attrs"
    appear
    enter-active-class="animated slideInRight"
    leave-active-class="animated slideOutRight">
    <div v-if="visible">
      <slot/>
    </div>
  </transition>
</template>

<script>
export default {
  name: 'SlideRight',

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
