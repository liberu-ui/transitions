<template>
    <transition v-bind="$attrs"
      appear
      enter-active-class="animated fadeInLeft"
      leave-active-class="animated fadeOutLeft">
      <div v-if="visible">
        <slot/>
      </div>
    </transition>
</template>

<script>
export default {
  name: 'FadeLeft',

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
