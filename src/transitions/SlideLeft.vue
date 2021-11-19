<template>
  <transition v-bind="$attrs"
    appear
    enter-active-class="animated slideInLeft"
    leave-active-class="animated slideOutLeft">
    <div v-if="visible">
      <slot/>
    </div>
  </transition>
</template>

<script>
export default {
  name: 'SlideLeft',

  data: () => ({
    visible: false,
  }),

  mounted() {
    this.visible = true;

    console.log('hit mounted SlideLeft')
  },

  unmounted() {
    this.visible = false;

    console.log('hit unmounted SlideLeft')
  }
};
</script>
