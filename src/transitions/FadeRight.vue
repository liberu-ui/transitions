<template>
  <transition v-bind="$attrs"
    appear
    enter-active-class="animated fadeInRight"
    leave-active-class="animated fadeOutRight">
    <div v-if="visible">
      <slot/>
    </div>
  </transition>
</template>

<script>
export default {
  name: 'FadeRight',

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
