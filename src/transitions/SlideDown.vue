<template>
    <transition v-bind="$attrs"
      appear
      enter-active-class="animated slideInDown"
      leave-active-class="animated slideOutUp">
      <div v-if="visible">
        <slot/>
      </div>
    </transition>
</template>

<script>
export default {
  name: 'SlideDown',

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
